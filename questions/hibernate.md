## ORM trong Hibernate là gì?
**ORM (Object Relational Mapping)** là kỹ thuật ánh xạ vật thể - quan hệ. Anh có thể hiểu đơn giản nó là một "cây cầu" giúp chuyển đổi dữ liệu từ các bảng trong cơ sở dữ liệu (Database) sang các đối tượng (Object) trong lập trình Java. Nó giúp việc tạo, sửa, xóa và lấy dữ liệu trở nên đơn giản hơn rất nhiều vì anh chỉ cần thao tác với Code Java thay vì viết SQL thô.

## Ưu điểm của Hibernate so với JDBC là gì?
* **Code sạch và dễ đọc:** Loại bỏ các đoạn code lặp đi lặp lại của JDBC, giúp code gọn gàng hơn.
* **HQL (Hibernate Query Language):** Đây là ngôn ngữ truy vấn hướng đối tượng, rất gần với Java. Nó giúp anh viết truy vấn mà không cần quan tâm Database bên dưới là MySQL hay Oracle (không phụ thuộc vào loại DB).
* **Quản lý giao dịch (Transaction):** JDBC bắt anh phải tự viết code `commit` và `rollback` thủ công, còn Hibernate tự động xử lý việc này.
* **Xử lý ngoại lệ:** Hibernate bao bọc các lỗi phức tạp của JDBC thành các lỗi dễ hiểu, giúp anh không phải viết quá nhiều khối `try-catch`.
* **Tính năng đặc biệt:** Hỗ trợ các tính năng của lập trình hướng đối tượng (OOP) như kế thừa, quan hệ giữa các bảng và Collection (List, Set...) - điều mà JDBC không làm được.

## Các Interface quan trọng của Hibernate Framework?
Các "khớp nối" quan trọng nhất gồm:
* **Configuration:** Cấu hình hệ thống.
* **SessionFactory:** Nhà máy tạo ra các Session (thường mỗi dự án chỉ có 1 cái).
* **Session:** Giữ kết nối giữa Java và Database (dùng để lưu/xóa dữ liệu).
* **Criteria:** Dùng để tạo các câu truy vấn động.
* **Query:** Thực thi các câu lệnh truy vấn.
* **Transaction:** Quản lý các phiên giao dịch.

## Session trong Hibernate là gì?
**Session** là một đối tượng duy trì kết nối giữa ứng dụng Java và Database. Nó cung cấp các phương thức để làm việc với dữ liệu như: `persist()` (lưu), `get()` (lấy), `update()` (cập nhật), `delete()` (xóa).

## SessionFactory là gì?
Đây là lớp "nhà máy" dùng để tạo ra các đối tượng Session dựa trên các tham số cấu hình. Thông thường, một ứng dụng chỉ nên có một `SessionFactory` duy nhất. Nó không thể thay đổi sau khi đã tạo và chứa các thông tin quan trọng (metadata) về việc ánh xạ dữ liệu.

## Lazy Loading (Tải chậm) là gì?
Đây là tính năng giúp tăng hiệu năng bằng cách **chỉ tải dữ liệu khi thực sự cần đến**. 
*Ví dụ:* Khi anh lấy thông tin một "Lớp học", Hibernate chưa tải danh sách "Học sinh" ngay. Chỉ khi nào anh gọi đến `lopHoc.getDanhSachHocSinh()`, dữ liệu học sinh mới được truy vấn từ Database.

## Sự khác biệt giữa Cache cấp 1 và Cache cấp 2?

| Đặc điểm | Cache cấp 1 (First Level) | Cache cấp 2 (Second Level) |
| :--- | :--- | :--- |
| **Phạm vi** | Chỉ nằm trong 1 **Session**. Không chia sẻ được giữa các Session khác nhau. | Nằm ở cấp **SessionFactory**. Tất cả các Session đều dùng chung được. |
| **Mặc định** | Luôn luôn bật, không tắt được. | Mặc định tắt, phải cấu hình mới dùng được. |
| **Vòng đời** | Mất đi ngay khi đóng Session. | Sống suốt vòng đời ứng dụng, chỉ mất khi khởi động lại app. |

## Khái niệm Kế thừa (Inheritance Mapping)?
Java có tính kế thừa (ví dụ: Học sinh kế thừa từ Người), nhưng Database thì chỉ có các bảng phẳng, không có khái niệm kế thừa. Hibernate giải quyết vấn đề này bằng các chiến lược:
* **Single Table:** Tất cả các lớp cha/con dùng chung 1 bảng duy nhất.
* **Table Per Class:** Mỗi lớp con có 1 bảng riêng.
* **Joined Table:** Lớp cha 1 bảng, lớp con 1 bảng, liên kết với nhau bằng khóa ngoại.

## Các Annotation (chú thích) phổ biến?
* `@Entity`: Đánh dấu class này là một bảng trong DB.
* `@Table`: Tên bảng tương ứng trong DB.
* `@Id`: Đánh dấu đây là khóa chính.
* `@GeneratedValue`: Cách tự động sinh số thứ tự (ID).
* `@Column`: Tên cột trong bảng.
* `@OneToOne`, `@OneToMany`...: Định nghĩa các mối quan hệ giữa các bảng.

## Khác biệt giữa get() và load()?

| get() | load() |
| :--- | :--- |
| Lấy dữ liệu ngay lập tức khi gọi hàm. | Trả về một đối tượng "giả" (proxy), chỉ lấy dữ liệu khi thực sự truy cập vào thuộc tính. |
| Truy vấn Database mỗi khi gọi. | Chỉ truy vấn khi thực sự cần (Lazy Loading). |
| Nếu không thấy dữ liệu -> trả về `null`. | Nếu không thấy dữ liệu -> báo lỗi `ObjectNotFoundException`. |
| Dùng khi không chắc chắn dữ liệu có tồn tại hay không. | Dùng khi biết chắc chắn dữ liệu đang nằm trong DB. |

## Criteria API là gì?
Đây là cách tạo câu lệnh truy vấn bằng Code Java (hướng đối tượng) thay vì viết chuỗi HQL. Nó cực kỳ mạnh mẽ khi anh cần xây dựng các bộ lọc tìm kiếm động (ví dụ: người dùng chọn lọc theo tên thì thêm điều kiện tên, chọn theo tuổi thì thêm điều kiện tuổi).

## HQL là gì?
**HQL** là ngôn ngữ truy vấn của Hibernate. Nó giống SQL nhưng thay vì viết tên Bảng (`table_name`), anh viết tên Class Java. Điều này giúp anh đổi Database thoải mái mà không cần sửa lại câu lệnh truy vấn.

## Hibernate có hỗ trợ SQL thuần (Native SQL) không?
**Có.** Anh có thể dùng hàm `createSQLQuery()` để viết các câu lệnh SQL y hệt như khi anh thao tác trực tiếp trên MySQL Workbench.

## Vấn đề N+1 SELECT là gì?
Đây là một lỗi về hiệu năng. 
*Ví dụ:* Anh muốn lấy 100 danh mục sản phẩm (1 câu query). Với mỗi danh mục, anh lại tốn thêm 1 câu query để lấy tên các sản phẩm bên trong. Tổng cộng anh tốn 1 + 100 = 101 câu query. Điều này làm ứng dụng chạy rất chậm.

## Cách giải quyết vấn đề N+1?
* Sử dụng **Batch fetching** (Lấy dữ liệu theo lô).
* Sử dụng **Join fetching** (Dùng lệnh Join để lấy hết dữ liệu trong 1 câu query duy nhất).
* Tắt Lazy loading ở những nơi cần thiết.

## Chiến lược Single Table là gì?
Là cách lưu toàn bộ sơ đồ kế thừa vào **duy nhất một bảng**. Hibernate dùng một cột đặc biệt (Discriminator) để phân biệt dòng nào thuộc về lớp nào. Đây là cách có hiệu năng tốt nhất vì không cần thực hiện lệnh Join giữa các bảng.

## Chiến lược Table Per Class là gì?
Mỗi lớp (kể cả lớp cha và lớp con) đều có bảng riêng trong Database.

## Named SQL Query là gì?
Là việc anh đặt tên cho một câu lệnh truy vấn và lưu nó lại (thường dùng Annotation `@NamedQuery` trên đầu Class). Khi cần dùng, anh chỉ cần gọi tên đó ra thay vì viết lại cả câu lệnh. Nó giống như việc đặt "biệt danh" cho câu truy vấn để tái sử dụng nhiều lần.
