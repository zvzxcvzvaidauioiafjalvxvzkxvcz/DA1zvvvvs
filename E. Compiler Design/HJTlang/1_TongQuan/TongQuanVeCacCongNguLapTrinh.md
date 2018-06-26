Các khái niệm cần tìm hiểu. Chỉ có khái niệm không có demo
====================================
 
  - Lịch sử ra đời
  
  - Tính năng
  
  - Ưu nhược điểm

Java
===============================

# I. Lịch sử ra đời

  - `Java` là một ngôn ngữ lập trình hướng đối tượng (`OOP`) và dựa trên các lớp (`class`). 
  
  - Khác với phần lớn ngôn ngữ lập trình thông thường, thay vì biên dịch mã nguồn thành mã máy hoặc thông dịch mã nguồn khi chạy, Java được thiết kế để biên dịch mã nguồn thành `bytecode`, `bytecode` sau đó sẽ được `môi trường thực thi (runtime environment)` chạy.

  - Trước đây, Java chạy chậm hơn những ngôn ngữ dịch thẳng ra mã máy như C và C++, nhưng sau này nhờ công nghệ `biên dịch tại chỗ - Just in time compilation`, khoảng cách này đã được thu hẹp, và trong một số trường hợp đặc biệt Java có thể chạy nhanh hơn

  - Java chạy nhanh hơn những ngôn ngữ thông dịch như `Python, Perl, PHP` gấp nhiều lần. Java chạy tương đương so với `C#`

  - Java được khởi đầu bởi James Gosling và bạn đồng nghiệp ở `Sun Microsystems` năm 1991

  - Tháng 04/2011, công ty `Sun Microsystems` tiếp tục cho ra bản JDK 1.6.24.

  -  Môi trường thực thi của `Sun Microsystems` hiện hỗ trợ `Sun Solaris, Linux, Mac OS, FreeBSD & Windows`

  - Một số công ty, tổ chức cũng như cá nhân khác cũng phát triển môi trường thực thi Java cho những hệ điều hành khác như `BEA, IBM, HP`.... Trong đó đáng nói đến nhất là `IBM Java Platform` hỗ trợ `Windows, Linux, AIX & z/OS`.

  - Có 5 mục tiêu chính trong việc xây dựng ngôn ngữ Java:

    + Đơn giản, hướng đối tượng và quen thuộc.
    
    + Mạnh mẽ và an toàn.
    
    + Kiến trúc trung lập và di động.
    
    + Thực thi với hiệu suất cao.
    
    + Dịch ra bytecode, phân luồng và năng động.
    
    + Dễ sử dụng cho người dùng Java

# II. Các phiên bản Java và tính năng

### 1. JDK 1.0 (23 tháng 01, 1996)

   - Đây là phiên bản đầu tiên của Java với 1 số tính năng đơn giản và đã có AWT

### 2. JDK 1.2 (19 tháng 2 năm 1997)

   - Phiên bản cải tiến JDK 1.0 với các tính năng như sau: 

     + Mở rộng `công cụ AWT` về mô hình các sự kiện

     + `inner class`

     + `JavaBean`

     + `JDBC`

     + `RMI`

     + `Reflection` chỉ hỗ trợ `Introspection`, không có khả năng thay đổi trong thời gian chạy.

     + `JIT (Just In Time)` compiler trên nền tảng `Microsoft Windows`, sản xuất cho `JavaSoft` bởi `Symantec`

     + `Internationalization` and `Unicode` hỗ trợ từ `Taligent`
     

### 3. J2SE 1.2 (Playground) 08 tháng 12 năm 1998

   - Có tên là `J2SE (Java 2 Platform, Standard Edition)` thay thế JDK để phân biệt 2 nền tảng `J2EE (Java 2 Platform, Enterprise Edition)` và `J2ME (Java 2 Platform, Micro Edition)`

   - Đây là 1 sự phát triển vượt bậc của Java với  1520 classes trong 59 packages.

   - Với Playground Java có thêm các tính năng sau:

     + `strictfp` keyword

     + `Swing graphical API `

     + Sun's JVM đã trang bị JIT compiler lần đầu tiên

     + `Java Applet`

     + `Java IDL`, an `IDL` implementation for `CORBA` interoperability

     + `Collections framework`: Java đi đến thiên đường từ đây




### 4. J2SE 1.3 (Kestrel) 08 tháng 5 năm 2000

   - `HotSpot` JVM

   - `RMI` được sửa đổi để thương thích với `CORBA`

   - Bao gồm `Java Naming and Directory Interface (JNDI)` trong bộ thư viện (`previously available as an extension`)

   - `Java Platform Debugger Architecture (JPDA)`

   - `JavaSound`

   - `Synthetic proxy classes`


### 5. J2SE 1.4.0 (Merlin) 06 tháng 02, 2002

   - Thay đổi về ngôn ngữ:

     + `assert` keyword

   - Cải tiến bộ thư viện:

     + `Regular expressions ` 

     + `Exception chaining`

     + Internet Protocol version 6 (IPv6) support

     + Non-blocking I/O (Java) 

     + Logging API

     + `Image I/O API` đọc và viết các hình ảnh như `JPEG and PNG`

     + Phân tích cú pháp `Integrated XML` và bộ xử lý `XSLT`  (`JAXP`)

     + `Integrated security` và  `cryptography extensions` (JCE, JSSE, JAAS) 

     + Java Web Start framework

     + `Preferences API` (java.util.prefs)

     + 

### 6. J2SE 5 (1.5.0) (Tiger) 30 tháng 9 năm 2004

   - Phiên bản với 50 lần cập nhật và fix lỗi vì các cải tiến là quá vượt trội so với các phiên bản trước đó

   - Các tính năng nổi bậc:

     + Generics

     + Metadata (annotations)

     + Autoboxing / unboxing

     + Enumerations

     + Varargs

     + Foreach

     + multi-threaded

     + Static imports

### 7. Java SE 6 (còn gọi là Mustang), được công bố 11 tháng 12 năm 2006

  - Đây là phiên bản có số lần fix lỗi khá lớn. Tuy các lần fix lỗi không được công khai nhưng có thời 
  gian ở lần fix cuối cùng là 2018-04-17

  - Đây là phiên bản mở rộng Java 5 và có các tính năng tương tự Java 5. Nhưng được hỗ trợ mạnh mẽ hơn

### 8. Java SE 7 (còn gọi là Dolphin), được bắt đầu từ tháng 8 năm 2006 và công bố ngày 28 tháng 7 năm 2011.

  - String trong switch statement

  - Binary Literals

  - The try-with-resources

  - Caching Multiple Exceptions by single catch

  - Underscores in Numeric Literals

### 9. JDK 8, 18 tháng 3 năm 2014
  
  - Đây là phiên bản đạt cột mốc cực mạnh của Java (như cột mốc Java 5)

  - Java 8 có rất nhiều tính năng vượt trội cần phải quan tâm đó là:

     + Java 8 Date/Time API
     
     + Lambda Expressions
     
     + Method References
     
     + Functional Interfaces
     
     + Stream
     
     + Base64 Encode Decode
     
     + Default Method
     
     + forEach method
     
     + Collectors 
     
     + StringJoiner 
     
     + Optional class 
     
     + Nashorn JavaScript 
     
     + Parallel Array Sorting 
     
     + Type Inference  
     
     + Method Parameter Reflection 
     
     + Type annotations and repeating annotations 
     
     + Java JDBC Improvements 

     + Java IO Improvement 
     
     + Java Concurrency Improvement 



### 10. JDK 9, 21 tháng 9 năm 2017
   
   - Platform Module System (Project Jigsaw)

   - Interface Private Methods

   - Try-With Resources

   - Anonymous Classes

   - @SafeVarargs Annotation

   - Collection Factory Methods

   - Process API Improvement

   - New Version-String Scheme

   - JShell: The Java Shell (REPL)

   - Process API Improvement

   - Control Panel

   - Stream API Improvement

   - Installer Enhancement for Microsoft windows and many more

### 11. JDK 10, 20 tháng 3 năm 2018
   
   - Local Variable Type Inference

   - Time-Based Release Versioning

   - Garbage-Collector Interface

   - Parallel Full GC for G1

   - Heap Allocation on Alternative Memory Devices

   - Consolidate the JDK Forest into a Single Repository

   - Root Certificates

   - Experimental Java-Based JIT Compiler

   - Thread-Local Handshakes

   - Remove the Native-Header Generation Tool

### 12. JDK 11, 20 tháng 3 năm 2018


# III. Ưu nhược điểm

### 1. Ưu điểm:
   
   -  Hướng đối tượng
   
   - Đọc lập nền tảng
   
   - IDE mạnh như: IntellIJ idea,....
   
   - Cú pháp đơn giản dể hiểu
   
   - Lập trình ứng dụng, web, và đặc biệt là lập trình trên thiết bị di động (Android)
   
   - Mã nguồn mở dẫn đến được phát triển mạnh mẽ với số lượng framework khổng lồ
   
### 2. Nhược điểm:

   - Tốc độ chậm do biên dịch rồi mới thông dịch sang mã máy tuy nhiên có thể chấp nhận được
   


C
===============================

# I. TỔng quan 

  - Ngôn ngữ lập trình C là một ngôn ngữ mệnh lệnh được phát triển từ đầu thập niên 1970 bởi Dennis Ritchie để dùng trong hệ điều hành UNIX

  - C là ngôn ngữ rất có hiệu quả và được ưa chuộng nhất để viết các phần mềm hệ thống, mặc dù nó cũng được dùng cho việc viết các ứng dụng
  
  - C cũng thường được dùng làm phương tiện giảng dạy trong khoa học máy tính mặc dù ngôn ngữ này không được thiết kế dành cho người nhập môn.

  - C là một ngôn ngữ lập trình tương đối nhỏ gọn vận hành gần với phần cứng và nó giống với ngôn ngữ Assembler hơn hầu hết các ngôn ngữ bậc cao. 
  
  - C đôi khi được đánh giá như là "có khả năng di động", cho thấy sự khác nhau quan trọng giữa nó với ngôn ngữ bậc thấp như là Assembler, đó là việc mã C có thể được 
  dịch và thi hành trong hầu hết các máy tính, hơn hẳn các ngôn ngữ hiện tại trong khi đó thì Assembler chỉ có thể chạy trong một số máy tính đặc biệt. 
  
  - C được xem là ngôn ngữ bậc trung.
  
# II. Tính năng

   - Một ngôn ngữ cốt lõi đơn giản, với các chức năng quan trọng chẳng hạn như là những hàm hay việc xử lý tập tin sẽ được cung cấp bởi các bộ thư viện các thủ tục.
   
   - Tập trung trên mẫu hình lập trình thủ tục, với các phương tiện lập trình theo kiểu cấu trúc.
   
   - Một hệ thống kiểu đơn giản nhằm loại bỏ nhiều phép toán không có ý nghĩa thực dụng.
   
   - Dùng ngôn ngữ tiền xử lý, tức là các câu lệnh tiền xử lý C, cho các nhiệm vụ như là định nghĩa các macro và hàm chứa nhiều tập tin mã nguồn (bằng cách dùng câu lệnh tiền xử lý dạng #include chẳng hạn).
   
   - Mức thấp của ngôn ngữ cho phép dùng tới bộ nhớ máy tính qua việc sử dụng kiểu dữ liệu pointer.
   
   - Số lượng từ khóa rất nhỏ gọn.
   
   - Các tham số được đưa vào các hàm bằng giá trị, không bằng địa chỉ.
   
   - Hàm các con trỏ cho phép hình thành một nền tảng ban đầu cho tính đóng và tính đa hình.
   
   - Hỗ trợ các bản ghi hay các kiểu dữ liệu kết hợp do người dùng từ khóa định nghĩa struct cho phép các dữ liệu liên hệ nhau có thể được tập hợp lại và được điều chỉnh như là toàn bộ.
  
# III. Ưu nhược điểm

### 1. Ưu điểm:

   - Đây là ngôn ngữ gần với mã máy nhất nên tốc độ chỉ sau ASM
   
   - Với sự phát triển các trình dịch C, và với sự phức tạp của các CPU hiện đại có tốc độ cao, C đã dần thu nhỏ khác biệt về tốc độ này. 
   
   - Do các trình dịch, các thư viện và các phần mềm thông dịch của các ngôn ngữ bậc cao khác lại thường được tạo nên từ C.
   
   - Khá nhiều ngôn ngữ xây dựng từ C, đặc biệt là JS
   
### 2. Nhược điểm:

   + An toàn kiểu,
   
   + Tự động Thu dọn rác,
   
   + Các lớp hay các đối tượng cùng với các ứng xử của chúng (xem thêm OOP),
   
   + Các hàm lồng nhau,
   
   + Lập trình tiêu bản hay Lập trình phổ dụng,
   
   + Quá tải và Quá tải toán tử,
   
   + Các hỗ trợ cho đa luồng, đa nhiệm và mạng.
   
   
 
C++
===============================

# I. Tổng quan và lịch sử ra đời

### 1. Tổng quang
  - C++ là một loại ngôn ngữ lập trình. Đây là một dạng ngôn ngữ đa mẫu hình tự do có `kiểu tĩnh` và hỗ trợ `lập trình thủ tục`, `dữ liệu trừu trượng`, `lập trình hướng đối tượng`,
   và `lập trình đa hình`. 
   
  - C++ đã trở thành một trong những ngôn ngữ thương mại phổ biến nhất trong khi đó.
  
  - `Bjarne Stroustrup` của `Bell Labs` đã phát triển C++ trong suốt thập niên 1980 như là một bản nâng cao của ngôn ngữ C. 
  
  - Những bổ sung nâng cao bắt đầu với sự thêm vào của khái niệm lớp, tiếp theo đó là các khái niệm `hàm ảo`, `chồng toán tử`, `đa kế thừa`, `tiêu bản`, và `xử lý ngoại lệ`. 
  
  - Tiêu chuẩn của ngôn ngữ C++ đã được thông qua trong năm 1998 như là `ISO/IEC 14882:1998`. Phiên bản hiện đang lưu hành là phiên bản `C++14`, `ISO/IEC 14882:2014`. 
  
  - Hiện tại tiêu chuẩn mới nhất của `ngôn ngữ C++` là `C++14`, phát hành ngày `15/12/2014` (ghi theo định dạng ISO 8601 là 2014-12-15). Và C++ còn là ngôn ngữ được cải tiến từ C.
  
### 2. Lịch sử ra đời

   - `Stroustrup` đã bắt đầu làm việc với khái niệm lớp trong `1979`. Ý tưởng tạo ra một ngôn ngữ mới bắt nguồn từ kinh nghiệm lập trình khi mà ông viết luận án tiến sĩ. 
     
   - Năm 1983, thì tên C với các lớp được đổi thành C++. các chức năng mới được thêm vào bao gồm hàm ảo, quá tải hàm và toán tử, tham chiếu, hằng, khả năng kiểm soát bộ nhớ của lưu trữ tự do, nâng cao việc kiểm soát kiểu, và lệnh chú giải kiểu (//).
     
   - Năm 1985, tác phẩm The C++ Programming Language được xuất bản lần đầu tiên, cung cấp một tài liệu tham khảo quan trọng cho ngôn ngữ nhưng đó chưa là một tiêu chuẩn chính thức.
     
   - Năm 1989 phiên bản C++ 2.0 phát hành. Các tính năng mới bao gồm đa kế thừa, lớp trừu tượng, hàm tĩnh, hàm thành viên hằng, và thành viên bảo tồn.
     
   - Năm 1990, cuốn The Annotated C++ Reference Manual được xuất bản cung cấp nền tảng cho tiêu chuẩn tương lai.
     
   - Phiên bản xuất bản sau đó có thêm các chức năng tiêu bản, ngoại lệ, không gian tên, chuyển kiểu cho toán tử new, và kiểu Boolean.
     
   - Khi C++ hình thành, thì thư viện chuẩn hoàn thiện với nó. Thư viện C++ đầu tiên thêm vào là iostream.h cung cấp cơ sở để thay thế các hàm C truyền thống như là printf và scanf. Sàu này, trong những thư viện chuẩn quan trọng nhất được thêm vào là Thư viện Tiêu bản Chuẩn.
     
   - Sau nhiều năm làm việc, có sự cộng tác giữa ANSI và hội đồng tiêu chuẩn hoá C++ của ISO để soạn thảo tiêu chuẩn ISO/IEC 14882:1998. 
   Phiên bản tiêu chuẩn này được phát hành năm 1989, hội đồng tiếp tục xử lý các báo cáo trục trặc, và ấn hành một phiên bản sửa sai của chuẩn C++ trong năm 2003.
     
   - Không ai là chủ nhân của ngôn ngữ C++, nó hoàn toàn miễn phí khi dùng. Mặc dù vậy, các văn bản tiêu chuẩn thì không miễn phí.
  
# II. Các tính năng

  - So với C, C++ tăng cường thêm nhiều tính năng, bao gồm: `khai báo như mệnh đề`, `chuyển kiểu giống như hàm`, `new/delete`, `bool`, các kiểu `tham chiếu`, `const`, 
  các `hàm nội tuyến (inline)`, các `đối số mặc định`, `nạp chồng hàm`, `không gian tên (namespace)`, các lớp (bao gồm tất cả các chức năng liên quan tới lớp như kế thừa, 
  hàm `thành viên (phương pháp)`, `hàm ảo`, `lớp trừu tượng`, và `cấu tử`) , `nạp chồng toán tử`, `tiêu bản`, `toán tử phạm vi ::`, `xử lý ngoại lệ`, 
  và sự nhận dạng kiểu trong thời gian thi hành.
  
  - C++ còn tiến hành nhiều phép kiểm tra kiểu hơn C trong nhiều trường hợp.
    
  - Câu lệnh chú giải bắt đầu với `//` nguyên là một phần của `BCPL` được tái sử dụng trong C++.
  
  - Một số thành phần của C++ sau này đã được thêm vào C, bao gồm `const`, `inline`, khai báo biến trong vòng lặp for và chú giải kiểu C++ (sử dụng ký hiệu //). 
  Tuy nhiên, C99 cũng bổ sung thêm một số tính năng không có trong C++, ví dụ như `macro` với số đối số động.
  
  - Vì được phát triển từ C, trong C++, thuật ngữ đối tượng có nghĩa là vùng nhớ như được dùng trong C, chứ không phải là một phiên bản của lớp như được hiểu trong phần lớn ngôn ngữ lập trình hướng đối tượng khác

# III. Điểm mạnh và điểm yếu 

### 1. Điểm mạnh

### 2. Điểm yếu



C#
===============================

Python
===============================

PHP
===============================

JavaScript
===============================

Visual Basic .NET
===============================

Delphi/Object Pascal
===============================

Perl
===============================

Ruby
===============================

Swift
===============================

Assembly language
===============================

GO
===============================

R
===============================

Visual Basic
===============================

MATLAB
===============================

PL/SQL
===============================

Objective-C
===============================

Scratch
===============================