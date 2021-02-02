# reflection
 Reflection ngày 1/2/2021
#### 1.Abstract Class.
+ Lớp trừu tượng trước tiên nó chính là 1 lớp, nhưng nó được gọi là lớp trừu tượng bởi vì: – Lớp này sẽ chứa các phương thức trừa tượng. – Các lớp khác khi kế thừa lớp trừu tượng sẽ phải định nghĩa các phương thức trừu tượng ấy
+ Mức truy cập các abstract method phải ở public hoặc protected để lớp kế thừa có thể định nghĩa lại.
+ Không dùng từ khóa final cho khai báo abstract class và abstract method.
#### 2. Interface.
+ Interface là một khuôn mẫu iúp cho chúng ta tạo ra bộ khung cho một hoặc nhiều đối tượng và nhìn vào interface thì chúng ta hoàn toàn có thể xác định được các phương thức và các thuộc tính cố định (hay còn gọi là hằng) sẽ có trong đối tượng implement nó.
+ Interface không thể khởi tạo.
+ Interface không phải là một lớp đối tượng .
#### 3. Ưu điểm.
> - stract class
 + Có thể linh động các method. giống như một class thông thường.
 + Các class extend có thể override hoặc không override các method thường.
  > - Interface.
 + Có thể implements nhiều interface(tính đa hình).
 + Xây dựng được bộ khung mẫu mà các lớp phải follow theo.
 + Giúp quản lý tốt, nắm bắt được các chức năng phải có cho một đối tượng nào đó.
### 4. Nhược điểm:
> - Abstract class:
 + Không thể extend nhiều abstract class.
> - Interface:
+ Mỗi khi định nghĩa thêm tính năng, các class impelement nó đồng lọat phải thêm tính năng đó.
#### 5. Tại sao lại sử dụng abstract class và interface.
> - Sử dụng abstract để tránh tình trạng khai báo nhiều lớp mà mỗi lớp có những thuộc tính và phương thức tương tự nhau.
> - Sử dụng interface để giải quyết vấn đề đa kế thừa.
> - Sử dụng abstract class và interface giúp dễ mở rộng ứng dụng cũng như bảo trì code.
### 6. Khi nào sử dụng.
> - Khi một nhóm đối tượng có cùng bản chất kế thừa từ một class thì sử dụng abstract class.
> - Khi một nhóm đối tượng không có cùng bản chất nhưng chúng có hành động giống nhau thì sử dụng interface.
***



Reflection ngày 28/1/2021
+ Access modifier là các từ khóa được sử dụng để quy định mức độ
phạm vi (visibility) truy cập đến lớp và các thành phần của lớp
+ Data field encapsulation (bao gói trường dữ liệu) là hình thức hạn chế
quyền truy cập trực tiếp vào các thuộc tính của đối tượng bằng cách
sử dụng từ khoá private
+ Các phương thức cho phép thay đổi giá trị của thuộc tính được gọi là
setter, các phương thức cho phép lấy về giá trị của thuộc tính được
gọi là getter
+ Phương thức static còn được gọi là phương thức của lớp (class
method)
+ bài học hôm nay học được là sử dụng  và hiểu được Access modifier
+ khai báo lớp, sử dụng GET SET  
+ làm được các bài tập cơ bản 
+ tìm kiếm thêm kiến thức về xây dựng  UML 

Reflection ngày 27/1/2021
+ Từ khoá class được sử dụng để khai báo lớp
+ Từ khoá new được sử dụng để khởi tạo đối tượng
+ Phương thức khởi tạo (constructor) là phương thức giúp khởi tạo các
đốitượng
+ Các phương thức cho phép thay đổi giá trị của thuộc tính được gọi
là setter, các phương thức cho phép lấy về giá trị của thuộc tính
được gọi là getter
+ Access modifier là các từ khoá được sử dụng để quy định mức độ
truy cập đến lớp và các thành phần của lớp
+ Các mức truy cập:
+ public: có thể truy cập từ bất cứ đâu
+ private: các phương thức và thuộc tính chỉ được phép truy xuất trong cùng
một lớp
+ protected: các phương thức và thuộc tính được phép truy xuất trong cùng
một lớp và ở các lớp con (kế thừa)
+  Từ khoá this được sử dụng để đại diện cho đối tượng hiện tại

Reflection ngày 22/1/2021
+ Website là một tập hợp các trang web con có thể chứa văn bản, hình ảnh, âm thanh, video. Trang đầu tiên của website được gọi là trang chủ
+ có hai loại website :
+Website tĩnh là loại website cơ bản mà có thể tạo ra dễ dàng. Bạn không cần sử dụng tới các ngôn ngữ lập trình web như Java, PHP,là trang web sử dụng hoàn toàn ngôn ngữ HTML
+ Website động là tập hợp của những trang web mà nội dung có khả năng thay đổi. Sự thay đổi có thể là tùy theo thời gian, tùy theo người dùng,Sử dụng ngôn ngữ phía máy chủ như PHP, Java , Python để phát triển một website.
+ LAMP là từ viết tắt để chỉ một bộ công nghệ được ưa chuộng và sử dụng phổ biến dùng trong xây dựng các ứng dụng web. Tên gọi LAMP xuất phát từ các chữ cái đầu của các công nghệ thành phần, bao gồm: Linux (hệ điều hành), Apache (ứng dụng web server), MySQL (hệ quản trị cơ sở dữ liệu) và PHP (ngôn ngữ lập trình PHP,Perl và Python)
+ Apache Web Server:• Là phần mềm máy chủ dịch vụ web (Web Server)
+ MySQL là một hệ quản trị cơ sở dữ liệu quan hệ mã nguồn mở
+ Hệ quản trị CSDL có chức năng lưu trữ dữ liệu, bảo mật, cung cấp
công cụ để truy xuất dữ liệu và nhiều tính năng khác.

#Reflection ngày 26/1/2021
+ Mảng là cơ chế giúp lưu trữ nhiều giá trị trong cùng một biến
+ Các giá trị được lưu trong mảng thường là cùng loại
+Mảng nhiều chiều:
+ Mảng nhiều chiều là mảng có các phần tử là các mảng
 Có thể có mảng 2 chiều, 3 chiều, 4 chiều... hoặc nhiều hơn
 + Có thể sử dụng vòng lặp for và for-each để duyệt mảng
+ Có thể nhúng nội dung của một trang PHP vào trong trang PHP
khác bằng include,include_once,require,require_once

+ phân biệt required vs required_one
+ câu lênh requiresDùng để import một file PHP khác vào file hiện tại, lúc này file hiện tại có thể sử dụng mọi tài nguyên của file import đó.
+ câu lệnh required_one Lệnh này có chức năng chẳng khác gì lệnh require, tuy nhiên điểm khác biệt đó là lệnh require_once chỉ import đúng một lần, nghĩa là khi bạn sử dụng hai lệnh require_once cùng một file thì ở lệnh require_once thứ hai nó sẽ thấy là đã xử lý rồi nên nó sẽ không thực thi nữa.
+ Khác nhau giữa require và include:
+Nếu khi import một file bằng lệnh require thì nếu chương trình bị lỗi thì lập tức trình biên dịch sẽ dừng và xuất ra thông báo lỗi. Còn nếu sử dụng lệnh include thì đó chỉ là một cảnh báo nên chương trình vẫn chạy cho đến cuối chương trình.
