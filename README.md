# reflection
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
