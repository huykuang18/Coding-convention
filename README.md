## 1. Coding convention là gì?
+ Là tập hợp các quy tắc khi code mục đích để cho code dễ đọc, dễ hiểu từ đó dễ quản lý, phát triển hơn.
+ **coding convention** có các quy tắc chung:
  + **Quy tắc đặt tên:**
    + Tên biến, tên hàm được đặt theo dạng **camelCase** hoặc **snake_case**
    + Tên lớp đặt theo dạng **PascalCase**
    + Hằng số đặt theo dạng **UPPER_CASE**
    + Tên biến, tên lớp thường là danh từ, cụm danh từ
    + Tên hàm thường bắt đầu bằng động từ (thể hiện hành dộng)
  + **Quy tắc số lượng:**
    + Hàm không nên quá 30 dòng
    + Lớp không nên quá 500 dòng
    + Một hàm không được vượt quá 5 tham số, nên giữ ở mức <= 3
    + Khi khai báo, 1 dòng chỉ chứa 1 biến
    + Một dòng không nên dài quá 80 ký tự
    + Các câu lệnh lồng nhau tối đa 4 cấp
  + **Quy tắc xuống dòng:**
    + Nếu có dấu phẩy thì xuống dòng sau dấu phẩy
    + Xuống dòng theo từng cấp lồng nhau
    + Xuống dòng mới thì nên bắt đầu ở cùng cột với đoạn lệnh cùng cấp ở trên
## 2.Chuẩn viết code trong PHP
> PHP có một chuẩn viết code là PRS(PHP Standards Recommendation). Chuẩn này có các mức khác nhau, tùy vào môi trường làm việc sẽ yêu cầu những mức PSR khác nhau.
+ **Chuẩn PSR-0, PSR-4: chuẩn Autoloading**
  + Từ PHP 5.3, khi khai báo class phải khai báo namespace
  + Một namespace và class đầy đủ điều kiện phải có cấu trúc như sau:
    + `<Vendor Name> (<Namespace>) <Class Name>` 
  + Mỗi namespace phải có một namespace gốc `<Vendor Name>`
  + Mỗi namespace có thể chứa nhiều namespace con (**sub-namespace**)
+ **Chuẩn PSR-1: các chuẩn cơ bản**
  + Code phải được viết trong cặp thẻ `<?php ?>` hoặc `<?= ?>`
  + Code chỉ được sử dụng UTF-8 không có BOM (Byte Order Mark)
  + Một file PHP chỉ nên làm 1 nhiệm vụ duy nhất, tránh chồng chéo (gọi là **side effect**)
  + Namespace và class phải tuân theo chuẩn PSR "autoloading" [PSR-0, PSR-4]
  + Tên class phải được khai báo theo dạng **PascalCase**
  + Hằng số phải viết theo dạng **UPPER_CASE**
  + Tên phương thức đặt theo dạng **camelCase**
+ **Chuẩn PSR-2: chuẩn viết code**
  + Code phải tuân thủ PSR-1 và PSR-0
  + Code sử dụng 4 dấu cách (spaces) để thụt lề, không dùng tab
  + Trên 1 dòng không vượt quá 120 ký tự, nên có từ 80 ký tự trở xuống
  + Sau khi khai báo `namespace` phải có 1 dòng trắng và sau khi khai báo `use` cũng phải có 1 dòng trắng
  + Dấu mở `{` của class hay hàm phải xuống dòng, và dấu đóng `}` phải ở dưới phần thân của class
  + Phạm vi truy cập (`public`, `protected`, `private`) phải được khai báo ở tất cả các thuộc tính và phương thức; `abstract` và `final` phải khai báo trước phạm vi truy cập, `static` phải khai báo sau phạm vi truy cập
  + **Control Structures**(if, else, elseif, for,...) phải có 1 dấu cách(space) đằng sau nó. Phương thức và hàm thì không cần
  + Dấu ngoặc mở `{` cho **control structure** phải trên cùng dòng, còn dấu ngoặc đóng `}` phải nằm ở dưới phần thân 1 dòng
  + Trong phần điều kiện của **control structure** `()` không được có khoảng trắng (space) ở ngay sau ngoặc mở `(` và ngay trước ngoặc đóng `)`
