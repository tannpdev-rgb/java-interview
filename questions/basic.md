-----

# Basic Java Interview Questions

  + [1. What is Java? What are the features of Java?](https://www.google.com/search?q=%231-what-is-java-what-are-features-of-java)
  + [2. What are the OOPs concepts?](https://www.google.com/search?q=%232-what-are-the-oops-concepts)
  + [3. What are different access modifiers in Java?](https://www.google.com/search?q=%233-what-are-different-access-modifiers-in-java)
  + [4. What is the meaning of SOLID?](https://www.google.com/search?q=%234-what-is-the-meaning-of-solid)
  + [5. What are primitive data types?](https://www.google.com/search?q=%235-what-are-primitive-data-types)
  + [6. Order of execution of Initialization blocks and Constructors in Java](https://www.google.com/search?q=%236-order-of-execution-of-initialization-blocks-and-constructors-in-java)
  + [7. Differences between Lambda Expressions and Closures in Java?](https://www.google.com/search?q=%237-differences-between-lambda-expressions-and-closures-in-java)
  + [8. Give the list of Java Object class methods](https://www.google.com/search?q=%238-give-the-list-of-java-object-class-methods)
  + [9. What is the difference between atomic, volatile, synchronized?](https://www.google.com/search?q=%239-what-is-the-difference-between-atomic-volatile-synchronized)
  + [10. Explain object finalization](https://www.google.com/search?q=%2310-explain-object-finalization)
  + [11. What is Serialization in Java?](https://www.google.com/search?q=%2311-what-is-serialization-in-java)
  + [12. Concept of Java Cloning](https://www.google.com/search?q=%2312-concept-of-java-cloning)
  + [13. StringBuffer vs StringBuilder](https://www.google.com/search?q=%2313-stringbuffer-vs-stringbuilder)
  + [14. Name some of the parsers which are commonly used to parse XML documents](https://www.google.com/search?q=%2314-name-some-of-the-parsers-which-are-commonly-used-to-parse-xml-documents)
  + [15. What New Features Were Added in Java 8?](https://www.google.com/search?q=%2315-what-new-features-were-added-in-java-8)
  + [16. What New Features Were Added in Java 11?](https://www.google.com/search?q=%2316-what-new-features-were-added-in-java-11)
  + [17. What Is a Lambda Expression and What Is It Used For?](https://www.google.com/search?q=%2317-what-is-a-lambda-expression-and-what-is-it-used-for)
  + [18. What Is an Exception?](https://www.google.com/search?q=%2318-what-is-an-exception)
  + [19. How to Generate OutOfMemoryError and StackOverflowException?](https://www.google.com/search?q=%2319-how-to-generate-outofmemoryerror-and-stackoverflowexception)
  + [20. What Are Annotations? What Are Their Typical Use Cases?](https://www.google.com/search?q=%2320-what-are-annotations-what-are-their-typical-use-cases)
  + [21. What is immutable class?](https://www.google.com/search?q=%2321-what-is-immutable-class)

## 1\. What is Java. What are features of Java?

Java là một ngôn ngữ lập trình bậc cao và độc lập nền tảng.

  + Java là ngôn ngữ hướng đối tượng. Tuy nhiên, mọi thứ (ngoại trừ các kiểu dữ liệu cơ bản) đều là đối tượng trong Java.
  + **Độc lập nền tảng:** Một chương trình duy nhất có thể chạy trên các nền tảng khác nhau mà không cần bất kỳ sự sửa đổi nào.
  + **Hiệu suất cao:** Trình biên dịch JIT (Just In Time) cho phép hiệu suất cao trong Java. JIT chuyển đổi bytecode thành ngôn ngữ máy và sau đó JVM bắt đầu thực thi.
  + **Đa luồng (Multi-threaded):** Chúng ta có thể viết các chương trình Java xử lý nhiều tác vụ cùng một lúc bằng cách định nghĩa nhiều luồng.
  + Java không hỗ trợ đa kế thừa thông qua lớp. Nó có thể đạt được thông qua các Interface (giao diện).
  + **Bảo mật:** Java bảo mật vì nó không sử dụng các con trỏ (pointer) tường minh.
  + Java là một ngôn ngữ lập trình mạnh mẽ vì nó sử dụng quản lý bộ nhớ chặt chẽ và các khái niệm như Tự động thu gom rác (Garbage collection).

[back to the top](https://www.google.com/search?q=%23basic-java-interview-questions)

## 2\. What are the OOPs concepts?

Các khái niệm OOP bao gồm:

  + **Kế thừa (Inheritance)** + Kế thừa có nghĩa là một lớp có thể mở rộng từ một lớp khác để mã nguồn có thể được tái sử dụng. Lớp đã có sẵn được gọi là lớp Cha (Super class), trong khi lớp dẫn xuất được gọi là lớp con (Sub class). Kế thừa chỉ áp dụng cho các thành viên `public` và `protected`. Các thành viên `private` không thể được kế thừa.
  + **Đóng gói (Encapsulation)**
      + Bảo vệ mã nguồn khỏi các tác động bên ngoài và tăng khả năng bảo trì. Để đóng gói, chúng ta cần để tất cả các biến thực thể là `private` và tạo các hàm `setter/getter` cho chúng, điều này buộc người khác phải gọi các hàm setter thay vì truy cập dữ liệu trực tiếp.
  + **Đa hình (Polymorphism)**
      + Một đối tượng duy nhất có thể tham chiếu đến lớp cha hoặc lớp con tùy thuộc vào kiểu tham chiếu. Đa hình áp dụng cho việc ghi đè phương thức (overriding).
  + **Trừu tượng (Abstraction)**
      + Trừu tượng hóa trong lập trình hướng đối tượng có nghĩa là che giấu các chi tiết phức tạp bên trong nhưng chỉ để lộ ra các đặc tính và hành vi thiết yếu phù hợp với ngữ cảnh.
  + **Giao diện (Interface)**
      + Đa kế thừa không thể đạt được trong Java bằng lớp. Để khắc phục vấn đề này, khái niệm Interface đã được giới thiệu. Interface là một khuôn mẫu chỉ có các khai báo phương thức mà không có phần thực thi phương thức.

[back to the top](https://www.google.com/search?q=%23basic-java-interview-questions)

## 3\. What are different access modifiers in Java?

  + **Default:** Là phạm vi truy cập khi không có bất kỳ từ khóa xác định nào; các thành viên dữ liệu, lớp và phương thức có thể truy cập được trong cùng một package.
  + **Private:** Được đánh dấu bằng từ khóa `private`, chỉ có thể truy cập được trong chính lớp đó, thậm chí các lớp trong cùng package cũng không truy cập được.
  + **Protected:** Có thể truy cập được trong cùng một package hoặc các lớp con ở các package khác.
  + **Public:** Có thể truy cập được từ mọi nơi.

[back to the top](https://www.google.com/search?q=%23basic-java-interview-questions)

## 4\. What is the meaning of SOLID?

SOLID đại diện cho năm nguyên tắc trong Java bao gồm:

  + **S**: Single responsibility principle (Nguyên tắc đơn trách nhiệm). Một lớp chỉ nên có một và chỉ một nhiệm vụ duy nhất.
  + **O**: Open-closed principle (Nguyên tắc Đóng/Mở). Các thành phần phần mềm nên mở để mở rộng, nhưng đóng để sửa đổi. Trình duyệt là một ví dụ hoàn hảo về chức năng mở để mở rộng nhưng đóng để sửa đổi.
  + **L**: Liskov substitution principle (Nguyên tắc thay thế Liskov). Các kiểu con phải có thể thay thế hoàn toàn cho các kiểu cơ sở (cha) của chúng.
  + **I**: Interface segregation principle (Nguyên tắc phân tách giao diện). Khách hàng không nên bị buộc phải triển khai các phương thức không cần thiết mà họ sẽ không sử dụng.
  + **D**: Dependency inversion principle (Nguyên tắc đảo ngược phụ thuộc). Nó phụ thuộc vào sự trừu tượng, không phải vào sự cụ thể. Theo đó, module cấp cao không bao giờ được phụ thuộc vào bất kỳ module cấp thấp nào.
    *Ví dụ:* Bạn đi đến một cửa hàng địa phương và thanh toán bằng thẻ ghi nợ. Nhân viên thu ngân không quan tâm bạn đưa loại thẻ nào (Visa, Master...). Họ chỉ đơn giản là quẹt thẻ, vì hệ thống của họ phụ thuộc vào giao diện thanh toán thẻ nói chung.

[back to the top](https://www.google.com/search?q=%23basic-java-interview-questions)

## 5\. What are primitive data types?

  + byte - 1 byte (8 bits). Min -2^7 Max 2^7-1
  + short - 2 byte (16 bits). Min -2^15 Max 2^15-1
  + char - 2 byte (16 bits). 2^16-1
  + int - 4 byte (32 bits). Min -2^31-1 Max 2^31
  + long - 8 byte (64 bits). Min -2^63-1 Max 2^63
  + float - 4 byte (32 bits). Min -2^31-1 Max 2^31
  + double - 8 byte (64 bits). Min -2^63-1 Max 2^63
  + boolean - NA (thường là 1 byte)

[back to the top](https://www.google.com/search?q=%23basic-java-interview-questions)

## 6\. Order of execution of Initialization blocks and Constructors in Java.

  + Khối khởi tạo tĩnh (**Static initialization blocks**) sẽ chạy bất cứ khi nào lớp được nạp lần đầu tiên vào JVM.
  + Các khối khởi tạo (**Initialization blocks**) chạy theo đúng thứ tự mà chúng xuất hiện trong chương trình.
  + Khối khởi tạo thực thể (**Instance Initialization blocks**) được thực thi bất cứ khi nào lớp được khởi tạo và trước khi các hàm khởi tạo (constructors) được gọi. Chúng thường được đặt phía trên các hàm khởi tạo trong dấu ngoặc nhọn `{}`.

[back to the top](https://www.google.com/search?q=%23basic-java-interview-questions)

## 7\. Differences between Lambda Expressions and Closures in Java.

Java hỗ trợ biểu thức lambda nhưng không hỗ trợ hoàn toàn Closure. Một biểu thức lambda là một hàm ẩn danh và có thể được định nghĩa như một tham số. Closure giống như các đoạn mã hoặc khối mã có thể được sử dụng mà không cần phải là một phương thức hay một lớp. Nó có nghĩa là Closure có thể truy cập các biến không được định nghĩa trong danh sách tham số của nó và gán nó vào một biến.

[back to the top](https://www.google.com/search?q=%23basic-java-interview-questions)

## 8\. Give the list of Java Object class methods.

  + `clone()` - Tạo và trả về một bản sao của đối tượng này.
  + `equals()` - Cho biết liệu một đối tượng khác có "bằng" đối tượng này hay không.
  + `finalize()` - Được gọi bởi bộ thu gom rác trên một đối tượng khi hệ thống xác định không còn tham chiếu nào đến đối tượng đó.
  + `getClass()` - Trả về lớp thực thi (runtime class) của một đối tượng.
  + `hashCode()` - Trả về giá trị mã băm cho đối tượng.
  + `notify()` - Đánh thức một luồng đơn đang chờ trên màn hình (monitor) của đối tượng này.
  + `notifyAll()` - Đánh thức tất cả các luồng đang chờ trên màn hình của đối tượng này.
  + `toString()` - Trả về một chuỗi đại diện cho đối tượng.
  + `wait()` - Làm cho luồng hiện tại phải chờ cho đến khi một luồng khác gọi phương thức `notify()` hoặc `notifyAll()` cho đối tượng này.

[back to the top](https://www.google.com/search?q=%23basic-java-interview-questions)

## 9\. What is the difference between atomic, volatile, synchronized?

Về cơ bản, một thao tác sẽ đọc giá trị từ bộ nhớ, tăng nó lên và đưa ngược lại bộ nhớ. Điều này hoạt động ổn trong đơn luồng, nhưng trong thời đại đa lõi, đa CPU và bộ đệm đa cấp, nó sẽ không chính xác. Nó gây ra tình trạng **Race condition** (nhiều luồng đọc giá trị cùng lúc) và vấn đề về khả năng hiển thị (Visibility).

**Volatile**
Khai báo một biến là `volatile` có nghĩa là việc sửa đổi giá trị của nó sẽ ảnh hưởng ngay lập tức đến bộ nhớ lưu trữ thực tế của biến đó. Trình biên dịch không thể tối ưu hóa các tham chiếu đến biến này. Điều này đảm bảo rằng khi một luồng sửa đổi biến, tất cả các luồng khác sẽ thấy giá trị mới ngay lập tức.

**AtomicInteger** \`\`\`java
private AtomicInteger counter = new AtomicInteger();

public int getNextUniqueIndex() {
return counter.getAndIncrement();
}

````
Lớp `AtomicInteger` sử dụng các thao tác CPU cấp thấp CAS (compare-and-swap) mà không cần đồng bộ hóa (synchronization). Khai báo một biến atomic đảm bảo các thao tác trên biến đó xảy ra một cách nguyên tử, tức là tất cả các bước con của thao tác đều được hoàn thành trong luồng mà chúng được thực thi và không bị gián đoạn bởi các luồng khác.

**Synchronizing**
Đồng bộ hóa tất cả các truy cập vào một biến chỉ cho phép một luồng duy nhất tại một thời điểm truy cập biến đó, và buộc tất cả các luồng khác phải chờ cho đến khi luồng đang truy cập giải phóng quyền truy cập.

Việc đồng bộ hóa xảy ra trên một đối tượng. Gọi một phương thức `synchronized` của một lớp sẽ khóa đối tượng `this` của lời gọi đó. Các phương thức `static synchronized` sẽ khóa chính đối tượng Lớp (Class object).

Truy cập đồng bộ thường được triển khai bằng `monitor` hoặc `semaphore`. Đây là các cơ chế loại trừ tương hỗ (mutex) cấp thấp cho phép một luồng giành quyền kiểm soát độc quyền một biến hoặc khối mã.

[back to the top](#basic-java-interview-questions)

## 10. Explain object finalization

Được gọi bởi bộ thu gom rác (garbage collector) trên một đối tượng khi hệ thống xác định không còn tham chiếu nào đến đối tượng đó. Nếu một đối tượng không thể được truy cập từ bất kỳ đối tượng sống nào, điều đó có nghĩa là nó có thể được thu gom rác một cách an toàn.

[back to the top](#basic-java-interview-questions)

## 11. What is Serialization in Java?

**Serialization** (Tuần tự hóa) đối tượng trong Java là một quá trình được sử dụng để chuyển đổi Đối tượng sang định dạng nhị phân, định dạng này có thể được lưu trữ lâu dài vào đĩa hoặc gửi qua mạng đến bất kỳ máy ảo Java (JVM) nào khác đang chạy; quá trình ngược lại là tạo đối tượng từ luồng nhị phân được gọi là **deserialization**. Java cung cấp API Serialization bao gồm `java.io.Serializable`, `java.io.Externalizable`, `ObjectInputStream` và `ObjectOutputStream`, v.v.

`Serializable` là một **marker interface** (giao diện đánh dấu). Giao diện đánh dấu trong Java là các giao diện không có trường hoặc phương thức nào (interface rỗng).

Việc làm cho một lớp có thể tuần tự hóa rất dễ dàng, chỉ cần triển khai giao diện `java.io.Serializable` và JVM sẽ lo việc tuần tự hóa các đối tượng theo định dạng mặc định.

`serialVersionUID` được sử dụng để đảm bảo rằng cùng một lớp (đã được sử dụng trong quá trình Serialization) được nạp lại trong quá trình Deserialization. Nó được dùng để kiểm soát phiên bản của đối tượng.

Bạn có thể tùy chỉnh quá trình Serialization bằng cách định nghĩa phương thức `writeObject` và `readObject`. Để tránh tuần tự hóa một số biến, bạn có thể đánh dấu biến đó là `static` hoặc `transient`.

[back to the top](#basic-java-interview-questions)

## 12. Concept Of Java Cloning

Java hỗ trợ hai loại nhân bản: **Deep clone** (nhân bản sâu) và **Shallow clone** (nhân bản nông). Theo mặc định, nhân bản nông được sử dụng. Lớp Object có phương thức `clone()` thực hiện nhân bản nông. Nhân bản nông sao chép ít nhất có thể, giúp tiết kiệm bộ nhớ.
1) Nếu lớp chỉ có các thành viên kiểu dữ liệu nguyên thủy, một bản sao hoàn toàn mới của đối tượng sẽ được tạo ra.
2) Nếu lớp chứa các thành viên kiểu lớp (đối tượng), thì chỉ có các tham chiếu đối tượng đến các thành viên đó được sao chép, do đó cả bản gốc và bản sao đều tham chiếu đến cùng một đối tượng thành viên.

Trong **Deep copy**, toàn bộ đối tượng được sao chép. Bộ nhớ mới được cấp phát cho đối tượng và nội dung được sao chép sang. Khi thực hiện sao chép sâu, các tham chiếu mới được tạo ra cho các đối tượng bên trong.

[back to the top](#basic-java-interview-questions)

## 13. StringBuffer vs StringBuilder

`StringBuffer` được đồng bộ hóa (synchronized), còn `StringBuilder` thì không. `StringBuilder` nhanh hơn `StringBuffer` vì nó không tốn chi phí cho việc đồng bộ hóa.

[back to the top](#basic-java-interview-questions)

## 14. Name some of the parsers which are commonly used to parse XML documents.

+ **DOM Parser** - Phân tích tài liệu bằng cách tải toàn bộ nội dung của tài liệu và tạo cây phân cấp hoàn chỉnh của nó trong bộ nhớ. Chúng ta có thể phân tích, sửa đổi hoặc tạo tài liệu XML.
+ **SAX Parser** - Phân tích tài liệu dựa trên các trình kích hoạt sự kiện (event-based). Không tải toàn bộ tài liệu vào bộ nhớ. Thường dùng cho các tài liệu XML rất lớn. Chúng ta chỉ có thể xử lý theo chiều tiến tới (forward-only).
+ **StAX Parser** - Phân tích tương tự SAX, nhưng StAX là một **PULL API** trong khi SAX là một **PUSH API**. Điều này có nghĩa là với StAX, ứng dụng khách cần chủ động yêu cầu trình phân tích lấy thông tin khi cần, còn SAX sẽ tự động thông báo cho ứng dụng khi có thông tin.

[back to the top](#basic-java-interview-questions)

## 15. What New Features Were Added in Java 8?

Java 8 đi kèm với một số tính năng mới, quan trọng nhất là:

+ **Lambda Expressions** − một tính năng ngôn ngữ mới cho phép chúng ta xử lý các hành động như các đối tượng.
+ **Method References** − cho phép định nghĩa Lambda bằng cách tham chiếu trực tiếp đến tên phương thức.
+ **Optional** − lớp bọc đặc biệt dùng để biểu thị sự tồn tại hoặc vắng mặt của giá trị.
+ **Functional Interface** – giao diện có tối đa một phương thức trừu tượng; việc triển khai có thể được cung cấp bằng Lambda.
+ **Default methods** − cho phép thêm các phần thực thi đầy đủ vào giao diện bên cạnh các phương thức trừu tượng.
+ **Stream API** − một lớp iterator đặc biệt cho phép xử lý các tập hợp đối tượng theo phong cách lập trình hàm.
+ **Date API** − một API ngày tháng được cải tiến, bất biến, lấy cảm hứng từ JodaTime.

[back to the top](#basic-java-interview-questions)

## 16. What New Features Were Added in Java 11?

Java 11 mang đến các tính năng như:

+ Các phương thức mới cho lớp String: `isBlank`, `lines`, `strip`, `stripLeading`, `stripTrailing`, và `repeat`.
+ Phương thức File mới − các phương thức tĩnh `readString` và `writeString` từ lớp `Files`.
+ **HTTP client mới** − cải thiện hiệu suất tổng thể và hỗ trợ cả HTTP/1.1 và HTTP/2.
+ Hệ thống Modular (Modular System) – có từ Java 9.

[back to the top](#basic-java-interview-questions)

## 17. What Is a Lambda Expression and What Is It Used For?

Nói một cách đơn giản, một biểu thức lambda là một hàm mà chúng ta có thể tham chiếu và truyền đi như một đối tượng.

Hơn nữa, các biểu thức lambda đưa phong cách xử lý hàm vào Java, giúp việc viết mã trở nên gọn nhẹ và dễ đọc hơn. Chúng là sự thay thế tự nhiên cho các lớp ẩn danh (anonymous classes) và dùng để triển khai nội dòng (inline) các giao diện chức năng (functional interfaces).

[back to the top](#basic-java-interview-questions)

## 18. What Is an Exception?

Một **ngoại lệ** (exception) là một sự kiện bất thường xảy ra trong quá trình thực thi chương trình và làm gián đoạn luồng hướng dẫn bình thường của chương trình.
Từ khóa `throws` được dùng để chỉ ra rằng một phương thức có thể gây ra ngoại lệ. Từ khóa `throw` cho phép chúng ta chủ động ném ra một đối tượng ngoại lệ.
Chúng ta xử lý ngoại lệ bằng khối `try-catch-finally`.
+ `try`: Chứa khối mã có thể xảy ra lỗi.
+ `catch`: Thực thi nếu có ngoại lệ phù hợp xảy ra.
+ `finally`: Luôn được thực thi sau khi thoát khỏi khối `try`, dù có ngoại lệ hay không.
**Checked exception** phải được xử lý hoặc khai báo; trong khi **Unchecked exception** thì không bắt buộc.

[back to the top](#basic-java-interview-questions)

## 19. How to Generate OutOfMemoryError and StackOverflowException?

**OutOfMemoryError** (Lỗi tràn bộ nhớ Heap)
```java
List<long[]> list = new LinkedList<long[]>();
while (true) {
  list.add(new long[65536]); // Thêm liên tục cho đến khi hết bộ nhớ RAM dành cho Heap
}
````

**StackOverflowException** (Lỗi tràn bộ nhớ Stack do đệ quy quá sâu)

```java
public class StackOverflowErrorExample {
    public static void recursivePrint(int num) {
        System.out.println("Number: " + num);
        recursivePrint(++num); // Gọi đệ quy vô hạn
    }
    public static void main(String[] args) {
        StackOverflowErrorExample.recursivePrint(1);
    }
}
```

[back to the top](https://www.google.com/search?q=%23basic-java-interview-questions)

## 20\. What Are Annotations? What Are Their Typical Use Cases?

**Annotations** là các siêu dữ liệu (metadata) được gắn vào các thành phần của mã nguồn và không ảnh hưởng trực tiếp đến hoạt động của mã mà chúng tác động.

Các trường hợp sử dụng điển hình:

  + **Thông tin cho trình biên dịch** – trình biên dịch có thể phát hiện lỗi hoặc ẩn cảnh báo.
  + **Xử lý lúc biên dịch và triển khai** – các công cụ phần mềm có thể xử lý annotation để tạo mã, file cấu hình, v.v.
  + **Xử lý lúc thực thi (Runtime)** – có thể kiểm tra annotation lúc đang chạy để tùy chỉnh hành vi của chương trình.

[back to the top](https://www.google.com/search?q=%23basic-java-interview-questions)

## 21\. What is immutable class?

Đối tượng bất biến (**Immutable objects**) là những đối tượng mà trạng thái của chúng không thể thay đổi sau khi được tạo. Ví dụ: `String`, `Integer`. Các lớp bất biến an toàn trong đa luồng (thread-safe) vì trạng thái không thể thay đổi nên không gây ra xung đột khi truy cập song song.

Để tạo một lớp bất biến trong Java:

  + Khai báo lớp là `final` để không thể bị kế thừa.
  + Để tất cả các trường là `private` để ngăn truy cập trực tiếp.
  + Không cung cấp các phương thức `setter`.
  + Để tất cả các trường có thể thay đổi (mutable fields) là `final` để giá trị chỉ được gán một lần.
  + Khởi tạo tất cả các trường qua hàm khởi tạo thực hiện sao chép sâu (deep copy).
  + Thực hiện nhân bản đối tượng trong các phương thức getter để trả về một bản sao thay vì trả về tham chiếu đối tượng thực tế.

[back to the top](https://www.google.com/search?q=%23basic-java-interview-questions)
