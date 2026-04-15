-----
# Câu hỏi phỏng vấn Java cơ bản

  + [1. Java là gì? Các tính năng của Java?](https://www.google.com/search?q=%231-what-is-java-what-are-features-of-java)
  + [2. Các khái niệm OOP là gì?](https://www.google.com/search?q=%232-what-are-the-oops-concepts)
  + [3. Các phạm vi truy cập (Access Modifiers) trong Java?](https://www.google.com/search?q=%233-what-are-different-access-modifiers-in-java)
  + [4. Ý nghĩa của SOLID là gì?](https://www.google.com/search?q=%234-what-is-the-meaning-of-solid)
  + [5. Các kiểu dữ liệu nguyên thủy là gì?](https://www.google.com/search?q=%235-what-are-primitive-data-types)
  + [6. Thứ tự thực thi của khối khởi tạo và Hàm khởi tạo (Constructor)](https://www.google.com/search?q=%236-order-of-execution-of-initialization-blocks-and-constructors-in-java)
  + [7. Khác biệt giữa Lambda Expression và Closure trong Java?](https://www.google.com/search?q=%237-differences-between-lambda-expressions-and-closures-in-java)
  + [8. Danh sách các phương thức của lớp Object](https://www.google.com/search?q=%238-give-the-list-of-java-object-class-methods)
  + [9. Khác biệt giữa atomic, volatile và synchronized?](https://www.google.com/search?q=%239-what-is-the-difference-between-atomic-volatile-synchronized)
  + [10. Giải thích về việc dọn dẹp đối tượng (Finalization)](https://www.google.com/search?q=%2310-explain-object-finalization)
  + [11. Serialization trong Java là gì?](https://www.google.com/search?q=%2311-what-is-serialization-in-java)
  + [12. Khái niệm Cloning (Nhân bản đối tượng)](https://www.google.com/search?q=%2312-concept-of-java-cloning)
  + [13. So sánh StringBuffer và StringBuilder](https://www.google.com/search?q=%2313-stringbuffer-vs-stringbuilder)
  + [14. Tên một số bộ phân tích (Parser) phổ biến để xử lý tài liệu XML](https://www.google.com/search?q=%2314-name-some-of-the-parsers-which-are-commonly-used-to-parse-xml-documents)
  + [15. Những tính năng mới nào được thêm vào Java 8?](https://www.google.com/search?q=%2315-what-new-features-were-added-in-java-8)
  + [16. Những tính năng mới nào được thêm vào Java 11?](https://www.google.com/search?q=%2316-what-new-features-were-added-in-java-11)
  + [17. Lambda Expression là gì và dùng để làm gì?](https://www.google.com/search?q=%2317-what-is-a-lambda-expression-and-what-is-it-used-for)
  + [18. Ngoại lệ (Exception) là gì?](https://www.google.com/search?q=%2318-what-is-an-exception)
  + [19. Làm sao để tạo ra lỗi OutOfMemoryError và StackOverflowException?](https://www.google.com/search?q=%2319-how-to-generate-outofmemoryerror-and-stackoverflowexception)
  + [20. Annotation là gì? Các trường hợp sử dụng phổ biến?](https://www.google.com/search?q=%2320-what-are-annotations-what-are-their-typical-use-cases)
  + [21. Lớp bất biến (Immutable class) là gì?](https://www.google.com/search?q=%2321-what-is-immutable-class)

-----

## 1\. Java là gì. Các tính năng của Java?

Java là một ngôn ngữ lập trình bậc cao và độc lập nền tảng.

  + **Hướng đối tượng:** Mọi thứ trong Java đều là đối tượng (ngoại trừ các kiểu dữ liệu cơ bản).
  + **Độc lập nền tảng:** Một chương trình có thể chạy trên nhiều nền tảng khác nhau mà không cần sửa đổi.
  + **Hiệu suất cao:** Nhờ trình biên dịch JIT (Just In Time). JIT chuyển đổi bytecode thành ngôn ngữ máy để JVM thực thi.
  + **Đa luồng (Multi-threaded):** Cho phép viết chương trình xử lý nhiều tác vụ cùng lúc.
  + **Không hỗ trợ đa kế thừa qua lớp:** Nhưng có thể đạt được thông qua Interface.
  + **Bảo mật:** Java bảo mật vì không sử dụng con trỏ (pointer) trực tiếp.
  + **Mạnh mẽ:** Sử dụng quản lý bộ nhớ chặt chẽ và cơ chế thu gom rác tự động (Garbage Collection).

[quay lại đầu trang](https://www.google.com/search?q=%23basic-java-interview-questions)

## 2\. Các khái niệm OOP là gì?

Các khái niệm OOP bao gồm:

  + **Tính kế thừa (Inheritance):** Một lớp có thể mở rộng từ lớp khác để tái sử dụng mã nguồn. Lớp có sẵn gọi là lớp cha (Super class), lớp kế thừa gọi là lớp con (Sub class). Chỉ áp dụng cho các thành phần `public` và `protected`.
  + **Tính đóng gói (Encapsulation):** Bảo vệ mã nguồn và tăng khả năng bảo trì. Thực hiện bằng cách để các biến thực thể là `private` và tạo các hàm `getter/setter`.
  + **Tính đa hình (Polymorphism):** Một đối tượng có thể tham chiếu đến lớp cha hoặc lớp con tùy thuộc vào kiểu tham chiếu. Áp dụng cho việc ghi đè phương thức (overriding).
  + **Tính trừu tượng (Abstraction):** Che giấu các chi tiết thực thi phức tạp bên trong, chỉ đưa ra các đặc điểm và hành vi thiết yếu.
  + **Giao diện (Interface):** Giải quyết vấn đề không hỗ trợ đa kế thừa. Interface là một khuôn mẫu chỉ chứa khai báo phương thức mà không có phần thực thi.

[quay lại đầu trang](https://www.google.com/search?q=%23basic-java-interview-questions)

## 3\. Các phạm vi truy cập (Access Modifiers) trong Java?

  + **Default:** Truy cập được trong cùng một package.
  + **Private:** Chỉ truy cập được trong chính lớp đó.
  + **Protected:** Truy cập được trong cùng package hoặc các lớp con ở package khác.
  + **Public:** Truy cập được từ mọi nơi.

[quay lại đầu trang](https://www.google.com/search?q=%23basic-java-interview-questions)

## 4\. Ý nghĩa của SOLID là gì?

SOLID đại diện cho 5 nguyên tắc trong Java:

  + **S (Single responsibility):** Một lớp chỉ nên có một nhiệm vụ duy nhất.
  + **O (Open-closed):** Mở để mở rộng, nhưng đóng để sửa đổi (Ví dụ: Plugin trình duyệt).
  + **L (Liskov substitution):** Các lớp con phải có thể thay thế hoàn toàn cho lớp cha mà không làm hỏng chương trình.
  + **I (Interface segregation):** Không nên ép khách hàng triển khai các phương thức mà họ không dùng tới.
  + **D (Dependency inversion):** Phụ thuộc vào trừu tượng (Abstraction), không phụ thuộc vào cụ thể (Concretion). Module cấp cao không được phụ thuộc vào module cấp thấp.

[quay lại đầu trang](https://www.google.com/search?q=%23basic-java-interview-questions)

## 5\. Các kiểu dữ liệu nguyên thủy là gì?

  * **byte**: 1 byte (8 bits).
  * **short**: 2 bytes (16 bits).
  * **char**: 2 bytes (16 bits).
  * **int**: 4 bytes (32 bits).
  * **long**: 8 bytes (64 bits).
  * **float**: 4 bytes (32 bits).
  * **double**: 8 bytes (64 bits).
  * **boolean**: Thường là 1 byte.

[quay lại đầu trang](https://www.google.com/search?q=%23basic-java-interview-questions)

## 6\. Thứ tự thực thi của khối khởi tạo và Constructor.

  + Khối khởi tạo tĩnh (**Static blocks**) chạy khi lớp được nạp lần đầu vào JVM.
  + Các khối khởi tạo (**Initialization blocks**) chạy theo thứ tự xuất hiện trong chương trình.
  + Khối khởi tạo thực thể (**Instance blocks**) chạy mỗi khi lớp được khởi tạo và chạy trước khi Constructor được gọi.

[quay lại đầu trang](https://www.google.com/search?q=%23basic-java-interview-questions)

## 7\. Khác biệt giữa Lambda Expressions và Closures.

Java hỗ trợ Lambda nhưng không hỗ trợ Closure hoàn toàn theo nghĩa đen. Lambda là hàm ẩn danh có thể dùng làm tham số. Closure có thể truy cập các biến không nằm trong danh sách tham số của nó và gán nó vào một biến.

[quay lại đầu trang](https://www.google.com/search?q=%23basic-java-interview-questions)

## 8\. Danh sách các phương thức của lớp Object.

  + `clone()`: Tạo bản sao đối tượng.
  + `equals()`: So sánh bằng.
  + `finalize()`: Được gọi trước khi dọn rác.
  + `getClass()`: Trả về lớp thực tế của đối tượng.
  + `hashCode()`: Trả về mã băm.
  + `notify()`, `notifyAll()`: Đánh thức các luồng đang chờ.
  + `toString()`: Trả về chuỗi đại diện đối tượng.
  + `wait()`: Bắt luồng hiện tại chờ.

[quay lại đầu trang](https://www.google.com/search?q=%23basic-java-interview-questions)

## 9\. Khác biệt giữa atomic, volatile, synchronized?

  + **Race condition:** Xảy ra khi nhiều luồng cùng đọc/ghi giá trị tại một thời điểm.
  + **Volatile:** Đảm bảo khi một luồng sửa đổi biến, các luồng khác sẽ thấy giá trị mới ngay lập tức (không bị lưu cục bộ ở bộ đệm CPU).
  + **AtomicInteger:** Sử dụng các thao tác CPU cấp thấp (CAS - compare-and-swap) để đảm bảo tính nguyên tử mà không cần dùng `synchronized`.
  + **Synchronized:** Chỉ cho phép một luồng truy cập vào biến/khối code tại một thời điểm, các luồng khác phải chờ.

[quay lại đầu trang](https://www.google.com/search?q=%23basic-java-interview-questions)

## 10\. Giải thích về Object Finalization.

Được gọi bởi bộ thu gom rác (Garbage Collector) khi xác định không còn tham chiếu nào đến đối tượng. Khi một đối tượng không thể truy cập được nữa, nó có thể được dọn dẹp an toàn.

[quay lại đầu trang](https://www.google.com/search?q=%23basic-java-interview-questions)

## 11\. Serialization trong Java là gì?

Là quá trình chuyển đổi đối tượng thành định dạng nhị phân để lưu vào đĩa hoặc gửi qua mạng. Quá trình ngược lại gọi là **Deserialization**.

  + `Serializable` là một **Marker interface** (interface rỗng, không có phương thức).
  + `serialVersionUID`: Dùng để kiểm soát phiên bản đối tượng, đảm bảo cùng một lớp được nạp lại khi Deserialization.
  + Dùng từ khóa `transient` hoặc `static` để bỏ qua không Serialize một biến.

[quay lại đầu trang](https://www.google.com/search?q=%23basic-java-interview-questions)

## 12\. Khái niệm Cloning trong Java.

  + **Shallow cloning (Bản sao nông):** Mặc định trong Java. Nó chỉ sao chép các giá trị nguyên thủy; với các đối tượng bên trong, nó chỉ sao chép địa chỉ tham chiếu (cả bản gốc và bản sao dùng chung đối tượng bên trong).
  + **Deep copy (Bản sao sâu):** Tạo ra một bản sao hoàn toàn mới, cấp phát bộ nhớ mới cho cả các đối tượng bên trong.

[quay lại đầu trang](https://www.google.com/search?q=%23basic-java-interview-questions)

## 13\. StringBuffer vs StringBuilder.

  + `StringBuffer` hỗ trợ đồng bộ hóa (synchronized), an toàn cho đa luồng nhưng chậm hơn.
  + `StringBuilder` không hỗ trợ đồng bộ hóa, nhanh hơn và nên dùng cho đơn luồng.

[quay lại đầu trang](https://www.google.com/search?q=%23basic-java-interview-questions)

## 14\. Các bộ phân tích XML thường dùng.

  + **DOM Parser:** Tải toàn bộ tài liệu vào bộ nhớ dưới dạng cây phân cấp. Cho phép sửa đổi XML.
  + **SAX Parser:** Dựa trên sự kiện, không tải toàn bộ vào bộ nhớ. Phù hợp cho file XML cực lớn nhưng chỉ đọc theo một chiều.
  + **StAX Parser:** Giống SAX nhưng là **PULL API** (ứng dụng chủ động yêu cầu dữ liệu), giúp kiểm soát tốt hơn.

[quay lại đầu trang](https://www.google.com/search?q=%23basic-java-interview-questions)

## 15\. Tính năng mới trong Java 8?

  + **Lambda Expressions**: Xử lý hành động như đối tượng.
  + **Method References**: Tham chiếu trực tiếp đến phương thức bằng tên.
  + **Optional**: Lớp bọc để xử lý giá trị có thể null.
  + **Functional Interface**: Interface chỉ có duy nhất một phương thức trừu tượng.
  + **Default methods**: Cho phép viết phần thực thi ngay trong Interface.
  + **Stream API**: Xử lý Collection theo phong cách lập trình hàm.
  + **Date API**: Bộ thư viện xử lý thời gian mới (immutable).

[quay lại đầu trang](https://www.google.com/search?q=%23basic-java-interview-questions)

## 16\. Tính năng mới trong Java 11?

  + Các phương thức mới cho String: `isBlank`, `lines`, `strip`, `repeat`.
  + Phương thức mới cho File: `readString`, `writeString`.
  + **HTTP Client mới**: Hỗ trợ HTTP/2 và hiệu năng tốt hơn.

[quay lại đầu trang](https://www.google.com/search?q=%23basic-java-interview-questions)

## 17\. Lambda Expression là gì?

Đơn giản là một hàm mà chúng ta có thể tham chiếu và truyền đi như một đối tượng. Nó giúp code ngắn gọn, dễ đọc và thay thế cho các lớp ẩn danh (anonymous classes).

[quay lại đầu trang](https://www.google.com/search?q=%23basic-java-interview-questions)

## 18\. Ngoại lệ (Exception) là gì?

Là một sự kiện bất thường xảy ra khi thực thi chương trình làm gián đoạn luồng bình thường.

  + `throws`: Khai báo phương thức có thể gây ra ngoại lệ.
  + `throw`: Chủ động ném ra một ngoại lệ.
  + `try-catch-finally`: Khối lệnh để xử lý ngoại lệ. `finally` luôn luôn được chạy.
  + **Checked exception**: Phải được xử lý hoặc khai báo lúc biên dịch.
  + **Unchecked exception**: Không bắt buộc phải xử lý lúc biên dịch.

[quay lại đầu trang](https://www.google.com/search?q=%23basic-java-interview-questions)

## 19\. Tạo lỗi OutOfMemory và StackOverflow?

  + **OutOfMemoryError**: Tạo ra một danh sách vô hạn các mảng lớn cho đến khi hết RAM.
  + **StackOverflowError**: Gọi một hàm đệ quy không có điểm dừng cho đến khi hết bộ nhớ Stack.

[quay lại đầu trang](https://www.google.com/search?q=%23basic-java-interview-questions)

## 20\. Annotation là gì?

Là siêu dữ liệu (metadata) gắn vào mã nguồn. Chúng không ảnh hưởng trực tiếp đến hoạt động của code nhưng giúp trình biên dịch phát hiện lỗi, hỗ trợ các công cụ tạo file cấu hình hoặc tùy chỉnh hành vi lúc thực thi (Runtime).

[quay lại đầu trang](https://www.google.com/search?q=%23basic-java-interview-questions)

## 21\. Lớp bất biến (Immutable class) là gì?

Là lớp mà trạng thái của đối tượng không thể thay đổi sau khi tạo (Ví dụ: `String`, `Integer`).

  + Để tạo lớp bất biến: Khai báo lớp là `final`, các trường là `private final`, không có hàm `setter`, khởi tạo qua Constructor bằng cách sao chép sâu (deep copy).

[quay lại đầu trang](https://www.google.com/search?q=%23basic-java-interview-questions)


Hy vọng bản dịch này giúp anh Tấn ôn tập hiệu quả cho các buổi phỏng vấn sắp tới\! Nếu có phần nào cần giải thích sâu hơn về Code, anh cứ nhắn em nhé.
