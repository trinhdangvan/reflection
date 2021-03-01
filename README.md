# reflection
## Redlection 3/1/2021
#### Thủ tục lưu 
>- Là tập hợp các câu lệnh transact-SQL được xem như một khối lệnh đơn nhằm thực hiện một tác vụ cụ thể
>- Ưuđiểm: 
>- Tăng tính bảo mật
>_ Thực thi tiền biên dịch
>- Giảm thiểu lưu thông trong mô hình Client/Server
>- Khả năng sử dụng lạ
+ Câu lệnh EXECUTE được sử dụng để chạy các thủ tục do người dùng định nghĩa.
- Chỉ mục index:
  + Là bảng tra cuu đặc biệt mà DATABASE có thể sụng để tăng nhanh thời gian và hiệu suất thu nhập dữ liệu. Chỉ mục trong DATABASE là tương tự như một chỉ mục trong mục lục của cuốn sách.
  + Lưu ý: 
     + Các chỉ mục ko nên được sử dụng trong bảng nhỏ
     + Bảng thường xuyên có hoạt động update, insert.
     + Các chỉ  mục không nên sử dụng trên cột mà có chứa một số lượng lớn giá trị NULL
     + Không nên dùng trên các cột thường được sửa đổi.  
- Using view: 
  + Giúp cho hạn chế quyền truy cập vào dữ liệu theo cách mà người dùng có thể nhìn thấy và đôi khi sửa đổi chính xác những gì hộ cần.
  + Tóm tắt dữ liệu từ các bảng khác nhau có thể được sử dụng để tạo báo cáo.
  + Cú pháp tạo View:
    + CREATE VIEW view_name AS SELECT colum1, colum2...FROM table_name WHERE [condition]
- Store Procedure:
  + GIống như 1 chương trình con lưu trữ dữ liệu. 
  + GIúp cho tái sử dụng code một cách dễ dàng hơn
  + Cú pháp:
    + Create Procedure allrecords()
    +  BEGIN
    +  Select * from Student_info;
    +  END

***
## Reflection 26/2/2021.
#### Một số hàm thao tác với dữ liệu trong SQL.
+ 1 Count()
>- Hàm COUNT() trả về số bản ghi phù hợp với tiêu chí đã chỉ định.
>-  cú pháp :
>>- SELECT COUNT(tên_cột) FROM tên_bảng WHERE điều_kiện;
+ 2 AVG().
>- Hàm AVG() trả về giá trị trung bình của một cột số.
>- cú pháp : 
>> -SELECT AVG(tên_cột) FROM tên_bảng WHERE điều_kiện;
+ 3 SUM()
>- Hàm SUM() trả về tổng số của một cột số.
>- cú pháp:
>>- SELECT SUM(tên_cột) FROM tên_bảng WHERE điều_kiện;
+ 4 MIN().
>- Hàm MIN() trả về giá trị nhỏ nhất của cột đã chọn.
>- Cú pháp:
>>- SELECT MIN(tên_cột) FROM tên_bảng WHERE điều_kiện;
+ 5 MAX()
>- Hàm MAX() trả về giá trị lớn nhất của cột được chọn.
>- cú pháp:
>>- SELECT MAX(tên_cột) FROM tên_bảng WHERE điều_kiện;
***
## Reflection 25/2/2021.
#### Một số câu lệnh truy vấn trong SQL với MySQL.
+ 1 And và OR.
>- Toán tử AND trả về false nếu một trong hai biểu thức kết hợp được đánh giá là sai. 
> - cú pháp: WHERE boolean_expression_1 AND boolean_expression_2
>- Toán tử OR kết hợp hai hay nhiều biểu thức dạng boolean, chỉ cần một trong các điều kiện kết hợp là đúng thì kết quả là true. 
> - cú pháp: WHERE boolean_expression_1 OR boolean_expression_2
+ 2 Group by và mệnh đề HAVING.
>- mệnh đề group by là một phần không bắt buộc của câu lệnh SELECT, được sử dụng để nhóm các tập các hàng có cùng một giá trị vào thành một nhóm, mỗi nhóm đó chỉ trả về một hàng.
> - cú pháp : SELECT column1 FROM table-name GROUP BY column1;
>- Mệnh đề HAVING thay cho WHERE để hạn chế dữ liệu trả về trong tập kết quả. Mệnh đề WHERE dùng với các cột của bảng, tuy nhiên không dùng được với các hàm tập hợp. Mệnh đề HAVING dùng với các hàm tập hợp và đi sau GROUP BY.
> - Cú pháp : SELECT columnname(s) FROM tablename WHERE conditional GROUP BY column... HAVING conditional
+ 3 JOIN.
>- Mệnh đề JOIN được sử dụng để kết hợp các hàng từ hai hay nhiều bảng, dựa trên cột liên quan giữa chúng. JOIN gồm 3 loại cơ bản INNER JOIN, LEFT JOIN, RIGHT JOIN trong MySQL không hỗ trợ FULL JOIN.
> - cú pháp : SELECT column_name(s) FROM table1 INNER|LEFT|RIGHT JOIN table2 ON join_condition1 INNER|LEFT|RIGHT  JOIN table3 ON join_condition2 … WHERE conditions;
>- INNER JOIN khớp các hàng trong một bảng với các hàng trong các bảng khác và cho phép bạn truy vấn các hàng có chứa các cột từ cả hai bảng. 
>- LEFT JOIN cho phép bạn chọn các hàng từ cả hai bảng bên trái và bên phải khớp với tất cả các hàng từ bảng bên trái (table1) ngay cả khi không có kết quả tìm thấy trong bảng bên phải (table2).
>- RIGHT JOIN cho phép bạn chọn các hàng từ cả hai bảng bên trái và bên phải khớp với tất cả các hàng từ bảng bên phải (table2) ngay cả khi không có kết quả tìm thấy trong bảng bên phải (table1).
***
## Reflection 24/2/2021.
#### Thiết kế và tạo cơ sở dữ liệu.
+ 1 Mục đích :
> - Tìm ra một mô hình CSDL phù hợp với yêu cầu của khách hàng.
2 Các bước thực hiện.
> - b1: Xác định mục đích của CSDL.
> - b2: Tìm hiểu và tổ chức các thông tin cần lưu trữ.
> - b3: chia thông tin vào trong các bảng.
> - b4: Xác định trường dữ liệu của từng bảng.
> - b5: Khóa chính của các bảng.
> - b6: Mối quan hệ giữa các bảng.
> - b7: Làm mịn thiết kế.
> - b8: Áp dụng các quy tắc chuẩn hóa.
+ 3. Khóa chính (Primary key).
> - Dùng để xác định mẫu tin trong bảng là duy nhất.
> - Mỗi bảng chỉ tồn tại duy nhất một khóa chính.
> - Mỗi khóa chính có thể là một hay một nhóm các trường.
> - Giá trị khóa chính không được phép để null và giá trị đó là duy nhất trong bảng.
+ 4. Khóa ngoại (foreign key). 
> - Là tập hợp các thuộc tính trong bảng tham chiếu đến bảng khác.
> - bảng chứa khóa ngoại là bảng con còn bảng nó tham chiếu đến nó là bảng cha.
> - Giá trị của khóa ngoại nó cùng kiểu, cùng độ dài, cùng giá trị với cột của bảng nó tham chiếu đến.
+ 5. CHuẩn hóa dữ liệu.
+  Khái niệm.
> - Là kỹ thuật thiết kế CSDL tổ chức vào các bảng theo cách làm giảm dư thừa và phụ thuộc vào dữ liệu. 
+  Quy tắc 1NF.
> - Mỗi ô bảng chứa giá trị là nguyên tử (tức là không chia nhỏ hơn nữa).
> - Mỗi bản ghi trong bảng là duy nhất.
> - Không có giá trị của thuộc tính nào có thể tính toán được từ giá trị của thuộc tính khác.
+ Quy tắc 2NF. 
> - Phải là 1NF.
> - Loại bỏ những thuộc tính không khóa phụ thuộc vào một bộ phận khóa chính và tách chúng ra một bảng riêng có khóa chính là khóa mà chúng phụ thuộc vào.
+ Quy tắc 3NF.
> - Phải là 2NF.
> - Không có phụ thuộc chức năng bắc cầu tức là khi thay đổi một cột không khóa thì không có cột nào trong bảng giá trị bị thay đổi.
 ***
## Reflection 23/2/2021.
 ## 1  Cơ sở dữ liệu (database)
+  Khái niệm.
> - Cơ sở dữ liệu là một tập hợp các dữ liệu có tổ chức, thường được lưu trữ và truy cập từ hệ thống máy tính.
+ Mô hình dữ liệu.
> - Là cơ chế lưu trữ quản lý và truy vấn dữ liệu.
> - Một số mô hình.
 
> - CSDL phân cấp 
> - CSDL mạng.
> - CSDL đồ thị.
> - CSDL quan hệ.
> - CSDL đối tượng.
## 2. Hệ quản trị cơ sở dữ liệu (Database Management System - DBMS).
+ Khái niệm.
> - là phần mềm để quản lý cơ sở dữ liệu. 
+ Chức năng.
> -Các DBMS hiện tại cung cấp các chức năng khác nhau cho phép quản lý cơ sở dữ liệu và dữ liệu có thể được phân loại thành bốn nhóm chức năng chính: 
> - Định nghĩa dữ liệu: xác định kiểu, ràng buộc của dữ liệu.
> - Cập nhật dữ liệu : Chèn, sửa đổi và xóa dữ liệu thực tế.
> - Truy xuất : Cung cấp thông tin dữ liệu dưới dạng có thể sử dụng trực tiếp hoặc để xử lý thêm bởi các ứng dụng khác.
> - Quản lý dữ liệu : Bảo mật dữ liệu, theo dõi, sao lưu và có thể khôi phục thông tin đã bị hỏng do lỗi.
+ Hệ quản trị cơ sở dữ liệu quan hệ (RDBSM).
> - Hệ quản trị cơ sở dữ liệu quan hệ là hệ thống quản lý cơ sở dữ liệu dựa trên mô hình quan hệ hay hệ quản trị CSDL dùng để tạo lập, cập nhật và khai thác CSDL quan hệ là hệ quản trị CSDL quan hệ.
## 3. SQL (structured query language).
> - Ngôn ngữ truy vấn có cấu trúc là một loại ngôn ngữ máy tính để thao tác với h
> - Ngôn ngữ truy vấn có cấu trúc là một loại ngôn ngữ máy tính để thao tác với hệ quản trị cơ sở dữ liệu quan hệ (RDBMS).
## 3.so sánh DBMS VÀ RDBMS
+ DBMS
>- Viết tắt của	Hệ thống quản lý cơ sở dữ liệu
>- Dữ liệu được lưu trữ trong mô hình điều hướng.
>- Sửa đổi trong dữ liệu là phức tạp.	
>- Truy cập dữ liệu Tiêu thụ nhiều thời gian hơn.	
>- Khóa và chỉ mục	không sử dụng 
>- Cơ sở dữ liệu phân tán	không được hỗ trợ
+ RDBMS
>- Viết tắt của	Hệ thống quản lý cơ sở dữ liệu quan hệ
>- Dữ liệu được lưu trữ trong mô hình quan hệ (trong bảng).
>- Sửa đổi trong dữ liệu là dễ dàng và đơn giản.
>- Truy cập dữ liệu nhanh hơn so với DBMS.
>- Để thiết lập các khóa và chỉ mục mối quan hệ được sử dụng trong RDBMS.
>- Cơ sở dữ liệu phân tán	Được hỗ trợ bởi RDBMS.
****
## Reflection 22/2/2021.
### Biểu thức chính quy (regular Expression).
1. Khái niệm.
> - Miêu tả một chuỗi theo những quy tắc cú pháp nhất định.
> - là biểu thức được sử dụng để chỉ định một chuỗi các chuỗi cần thiết cho một mục đích cụ thể.
2. Tác dụng.
> - Tìm kiếm và thay thế một chuỗi con trong một chuỗi lớn.
> - Xác thực form (validate form).
> - Tiết kiệm thời gian lập trình.
3. Một số hàm thao tác với biểu thức chính quy trong php.
> - preg_match() : được dùng để kiểm tra, so khớp và lấy kết quả của việc so sánh chuỗi dựa vào biểu thức chính quy.
> - preg_match_all(): cũng tương tự hàm preg_match() ở trên , tuy nhiên hai hàm này khác nhau ở chỗ , hàm preg_match_all() sẽ trả về toàn bộ các giá trị được so sánh khớp, còn hàm preg_match() chỉ trả về giá trị đầu tiên được so sánh khớp.
> - pre_split: để chia nhỏ chuỗi thành mảng chứa các chuỗi con. 
> - preg_replace dùng để tìm kiếm và thay thế một chuỗi nào đó khớp với đoạn Regular Expression truyền vào. 
***
## Reflection 18/2/2021.
+ 1.Giải thuật sắp xếp.
>- Giải thuật sắp xếp là xác định cách sắp xếp dữ liệu theo một thứ tự nào đó. Sắp xếp theo thứ tự ở đây là sắp xếp theo thứ tự dạng số hoặc dạng chữ cái.
>- Giải thuật sắp xếp có tác dụng cho việc tối ưu tìm kiếm dữ liệu và sử dụng để biểu diễn dữ liệu dễ đọc hơn.
+ giải thuật sắp xếp In-place và not-in-place.
>- Những giải thuật mà không yêu cầu thêm bộ nhớ phụ và việc sắp xếp được tiến hành trong bộ nhó đã khai báo trước đó thì được gọi là In-place (vd: bubble sort, Insertion sort, selection sort).
>- Những giải thuật cần thêm bộ nhớ mà có thể lớn hơn hoặc bằng với số phần tử đang được sắp xếp thì gọi là not-in-place sorting (VD: merge sort).
+ Giải thuật sắp xếp cố định và sắp xếp so sánh.
>- Sau khi sắp xếp những phần tử có giá trị bằng nhau mà vị trí tương đối giữa chúng không thay đổi là sắp xếp cố định. và ngược lại thay đổi vị trí tương đối của 2 phần tử có giá trị bằng nhau thì là sắp xếp so sánh.
>
+ Giải thuật sắp xếp Adaptive và Non-adaptive.

>- khi sắp xếp nếu danh sách ban đầu có một số phần tử đã được sắp xếp, thì giải thuật dạng adaptive sẽ ghi nhận các phần tử này và sẽ cố gắng không thay đổi thứ tự của chúng.
>- giải thuật dạng non-adaptive sẽ không ghi nhận các phần tử đã được sắp xếp trước đó. Giải thuật loại này sẽ vấn cố gắng sắp xếp lại từng phần tử trong danh sách ban đầu.
+ 2 Bubble Sort (sắp xếp nổi bọt).
>- Giải thuật sắp xếp này được tiến hành dựa trên việc so sánh cặp phần tử liền kề nhau và tráo đổi thứ tự nếu chúng không theo thứ tự.
>-Giải thuật này không thích hợp sử dụng với các tập dữ liệu lớn khi mà độ phức tạp trường hợp xấu nhất và trường hợp trung bình là Ο(n2) với n là số phần tử.
+ 3 Insertion Sort (sắp xếp chèn).
>- Với cấu trúc dữ liệu mảng, chúng ta tưởng tượng là: mảng gồm hai phần: một danh sách con đã được sắp xếp và phần khác là các phần tử không có thứ tự. Giải thuật sắp xếp chèn sẽ thực hiện việc tìm kiếm liên tiếp qua mảng đó, và các phần tử không có thứ tự sẽ được di chuyển và được chèn vào vị trí thích hợp trong danh sách con (của cùng mảng đó).
> - Giải thuật này không thích hợp sử dụng với các tập dữ liệu lớn khi độ phức tạp trường hợp xấu nhất và trường hợp trung bình là Ο(n2) với n là số phần tử.
+ 4 Selection Sort ( Sắp xếp chọn).
> - Danh sách được chia thành hai phần, phần được sắp xếp (sorted list) ở bên trái và phần chưa được sắp xếp (unsorted list) ở bên phải.Phần tử nhỏ nhất được lựa chọn từ danh sách chưa được sắp xếp và được tráo đổi với phần bên trái nhất và phần tử đó trở thành phần tử của danh sách được sắp xếp. Tiến trình này tiếp tục cho tới khi toàn bộ từng phần tử trong danh sách chưa được sắp xếp đều được di chuyển sang mảng đã được sắp xếp.
> - Giải thuật này không phù hợp với tập dữ liệu lớn khi mà độ phức tạp trường hợp xấu nhất và trường hợp trung bình là O(n2) với n là số phần tử.
***
## Reflection 17/2/2021.
1. Tìm kiếm tuyến tính (Linear Search).
+ Khái niệm.
> - Tìm kiếm tuyến tính là hoạt động tìm kiếm liên tiếp được diễn ra qua tất cả từng phần tử. Mỗi phần tử đều được kiểm tra và trả về kết quả nếu tìm thấy phần tử đó nếu không thấy thì tìm kiếm đến hết dữ liệu.
+  Đặc điểm.
> - Có thể áp dụng với đối với bất kỳ mảng dữ liệu nào mà không cần phải sắp xếp theo một trật tự nhất định.
>- Độ phức tạp thời gian là O
3. Tìm kiếm nhị phân (Binary Search).
+ Khái niệm.
> - Binary search tìm kiếm một phần tử cụ thể bằng cách so sánh phần tử tại vị trí giữ nhất của tập dữ liệu. Nếu tìm thấy thì trả về kết quả chỉ mục của phần tử đó. Nếu phần tử cần tìm lớn hơn phần tử gìữa thì phần tử cần tìm nằm bên mảng con bên phải của phần tử giữa, nếu không thì sẽ tìm ở trong mảng con nằm ở bên trái phần tử giữa. Quá trình lặp lại cho đến khi tìm hết mọi phần tử trên mảng con này.
+  Đặc điểm.
> - Tìm kiếm nhị phân là một giải thuật tìm kiếm nhanh với độ phức tạp thời gian là O(log n).
> - Giải thuật tìm kiếm nhị phân làm việc trên nguyên tắc chia để trị (divide and conquer).
> - Dùng trong tìm kiếm dữ liệu đã được sắp xếp. 
 ***
Reflection 5/2/2021.
+ Hàm rewind() sẽ đặt lại vị trí con trỏ nội bộ của file về đầu file
+ Một danh sách liên kết đôi là một danh sách các node được liên kết với nhau theo cả hai hướng 
+ Heaps là một dạng câu trúc gần giống với tree trong đó mỗi node sẽ có giá trị lớn hơn hoặc bằng các node con của nó 
+ Arrays là cấu trúc dữ liệu trông đó lưu trữ các phần tử theo hình thức liên tiếp nhau ,các phần tử này được truy cập dưacj vào chỉ số của chúng 
+ Map là một cấu trúc dữ liệu trong đó ccác phần tử được quản lý theo cặp key-value (khó -giá trị)
***
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
