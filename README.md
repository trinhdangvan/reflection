# reflection
Reflection 4/2/2021.
#### 1. Stack.
+ khái niệm.
> - Là một loại cấu trúc dữ liệu tuyến tính hoạt động theo cơ chế first in/last out tức là dữ liệu vào trước thì sẽ lấy ra sau.
+ Ứng dụng trong thực tế.
> - Hiển thị nội dung history của trình duyệt.
> - Nội dung cập nhật ứng dụng.
#### 2. Queue.
+ Khái niệm.
> - Là một cấu trúc dữ liệu tuyến tính dạng danh sách trong đó việc thêm và lấy các phần tử được thực hiện theo quy tắc FIFO (first in/first out) tức là phần tử nào thêm trước thì sẽ được lấy ra trước.
+ Ứng dụng trong thực tế.
> - Danh sách khám bệnh ở bệnh viện.
> - Thứ tự đặt vé ở sân bay, rạp chiếu phim..
#### 3. Tree.
+ Khái niêm.
> - Là cấu trúc dữ liệu phi tuyến hoạt động theo nguyên tắc phân cấp, trong đó có mối quan hệ cha con giữa các node.
>- cấu trúc :
> - Root là nốt gốc tức là ko có cha.
> - Node mà ko có con thì gọi là leaf (nút lá).
> - Những node có chung cha gọi là sibling.
> - Đường kết nối giữa các node gọi là edges.
+ Đặc điểm.
> - Tốc độ truy xuất ở mức trung bình nó sẽ nhanh hơn dạng linked list và chậm hơn dạng Array list.
> - Tốc độ xử lý dữ liệu như thêm phần tử, xóa phần tử thì nhanh hơn dạng array list và chậm hơn linked list.
> - sử dụng tài nguyên bộ nhớ tốt hơn dạng list.
***
 Reflection ngày 3/2/2021
#### 1.Cấu trúc dữ liệu (data structures):
+ Khái niệm :
> - là hình thức tổ chức dữ liệu để sử dụng một cách hiệu quả.
+ Chức năng :
> - Lữu trữ dữ liệu.
> - Cung cấp các phương thức để thao tác với dữ liệu.
+  Thành phần chính trong một cấu trúc dữ liệu.
> - Container: là lớp chứa dữ liệu và cung cấp các phương thức để thao tác với dữ liệu.
> - Elements là các phần tử của dữ liệu.
+ Một số loại cấu trúc dữ liệu thông dụng.
> - Set nhóm phần tử không trùng nhau.
> - List Nhóm các phần tử có thể trùng nhau.
> - Stack Nhóm các phần tử theo trật tự vào trước ra sau.
> - Queue Nhóm các phần tử theo trật tự vào trước ra trước
> - Map Lưu dữ liệu theo cặp key - Value.
> - Tree Lưu dữ liệu theo quan hệ cha con
> - Grap lưu dữ liệu theo quan hệ mạng lưới.
### 2. ArrayList.
+ Khái niệm. 
>- Là một cấu trúc dữ liệu danh sách sử dụng mảng để lưu trữ dữ liệu.
+ Đặc điểm.
>- Truy xuất nhanh đến các phần tử (truy xuất theo index).
> - Các thao tác thêm sửa xóa không hiệu quả vì phải dịch chuyển lại các phần tử của mảng.
>
+ Hoạt động.
> - Thêm, sửa, xóa, tìm kiếm, duyệt..
### 3. Linked List
+ Khái niệm.
> - Là cấu trúc dữ liệu danh sách chứa các phần tử trong đó mỗi phần tử liên kết với phần tử tiếp theo của nó.
> - Mỗi phần tử bao gồm : Trường dữ liệu chứa giá trị thực sẽ được lưu trữ, xử lý và Trường liên kết giữ địa chỉ mục dữ liệu tiếp theo trong danh sách liên kết.
+ Đặc điểm.

> Ưu điểm:
> - Thao tác thêm xóa phần tử nhanh hơn loại Array list vì chỉ cần xác định phần tử trước đó và phần tử sau nó sau đó xóa trường liên kết của nó và cho trường liên kết của phần tử trước nó trỏ đến phần tử sau nó là xong.
>- Tốn ít tài nguyên bộ nhớ.
>
>  Nhược điểm:
> - vì các phần tử liên kết với nhau thành chuỗi như thế nên việc tìm kiếm một phần tử bất kỳ cũng đều phải duyệt từ phần tử đầu tiên trở đi làm mất nhiều thời gian
+ Các loại linked List.
> - Simple linked list chỉ duyệt các phần tử theo chiều về phía trước tức là các phần tử phía trước chỉ trỏ đến thằng sau nó.
> - Double linked list các phần tử có thể duyệt cả về trước lẫn về sau do các phần tử đều trở về cả phần tử trước nó và cả phần tử sau nó.
> - Circular linked list phần tử cuối cùng thì trỏ về phần tử đầu tiên.
+ Các hoạt động.
> - Thêm 1 phần tử.
> - Xóa một phần tử.
> - Duyệt.
> - Tìm kiếm.


***
 Reflection ngày 2/2/2021
#### 1. clean code.
+ clean code là những thuật ngữ chỉ những mã nguồn tốt.
 mã tốt là :
#### 2. mã tốt là :
+ Đơn giản (giải quyết vấn đề một cách ngắn gọn).
+ Trực tiếp ( giải quyết vấn đề chính xác không lòng vòng).
+ Dễ đọc.
+ Dễ cải tiến.
+ Các định danh thể hiện rõ nghĩa.
+ Không có mã bị trùng lặp.
+ Thể hiện được ý tưởng thiết kế.
#### 3.Nguyên lý SOLID.
+ Hiểu một cách đơn giản SOLID là 5 nguyên lý giúp lập trình viên phát triền phần mềm với kiến trúc tốt
+ Single responsibility principle là một class chỉ nên thực hiện một nhiệm vụ.
+ Open/closed principle là Có thể thoải mái mở rộng 1 class, nhưng không được sửa đổi bên trong class đó tức là mỗi khi ta muốn thêm chức năng,.. cho chương trình, chúng ta nên viết class mới mở rộng class cũ ( bằng cách kế thừa hoặc sở hữu class cũ) không nên sửa đổi class cũ.
+ Liskov Substitution Principle là trong một chương trình, các object của class con có thể thay thế class cha mà không làm thay đổi tính đúng đắn của chương trình
+ Interface Segregation Principle là thay vì dùng 1 interface lớn, ta nên tách thành nhiều interface nhỏ, với nhiều mục đích cụ thể.
+ Dependency inversion principle là các module cấp cao không nên phụ thuộc vào các modules cấp thấp và Interface (abstraction) không nên phụ thuộc vào chi tiết, mà ngược lại. (phần này hơi triết học).
#### 4. coding conventions.
+ Là những tập hợp các quy tắc chung khi lập trình nhằm làm code dễ đọc dễ hiểu do đó dễ quản lý và bảo trì.
+ Hạn chế dùng comment để giải thích code mà hãy cải thiện đoạn code của mình.
+ Chỉ dùng comment khi viết documentation cho thư viện, thông tin đính kèm cho class.

***

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
Reflection ngày 29/1/2021
#### Kế thừa
>- Những điều mới học 
+ Kế thừa là gì kế thừa là lớp con có thể kế thừa tất cả các thuộc tính và phương thức của lớp cha và có thêm các thuộc tính và phương thức mới 
+ Ghi đè là lớp con định nghĩa lại các thuộc tính và phương thức của lớp cha 
+ Có 3 dạng kế thừa là :
>- Single Một :lớp con kế thừa một lớp cha
>- Multilevel :Kế thừa từ lớp ông đến lớp cha rồi từ lớp cha đến lớp con 
>- Hierarchical :Một lớp cha kế thừa nhiều lớp con 
#### 3.Method overriding.
>- Method Overriding (ghi đè phương thức) là cơ chế cho phép lớp con định nghĩa lại các phương thức đã được định nghĩa trước đó ở lớp cha.
>- Phương thức override ở lớp con có cùng tên, cùng danh sách tham số và kiểu dữ liệu trả về so với phương thức ở lớp cha.
>- Phương thức ở lớp con phải có access modifier có level bằng hoặc cao hơn so với phương thức ở lớp cha.
#### 4. method overloading:
>-Nạp chồng (Overloading): Việc khai báo trong một lớp có nhiều thuộc tính, nhiều phương thức có cùng tên nhưng với các tham số khác nhau (khác kiểu dữ liệu,khác số lượng tham số).
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
