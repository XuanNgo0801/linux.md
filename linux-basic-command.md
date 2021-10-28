# Giới thiệu chung
- Khi vận hành hệ điều hành Linux, bạn cần sử dụng shell - một giao diện cho phép bạn truy cập vào các dịch vụ của hệ điều hành. Hầu hết các bản phân phối Linux đều sử dụng giao diện người dùng đồ họa (GUI) làm giao diện người dùng, chủ yếu là để mang lại sự dễ sử dụng cho người dùng của họ.
Điều đó đang được nói, bạn nên sử dụng giao diện dòng lệnh (CLI) vì nó mạnh mẽ và hiệu quả hơn. Các tác vụ yêu cầu quy trình nhiều bước thông qua GUI có thể được thực hiện trong vài giây bằng cách nhập lệnh vào CLI.
- Lưu ý: Shell của linux phân biệt chữ hoa, chữ thường.
____________________________
> ## Lệnh pwd
>
Sử dụng lệnh `pwd` để tìm ra đường dẫn của thư mục đang làm việc hiện tại mà bạn đang ở.  
Lệnh này sẽ trả về một đường dẫn tuyệt đối (đầy đủ), về cơ bản là đường dẫn của tất cả các thư mục bắt đầu bằng dấu gạch chéo (/ ) . Ví dụ về đường dẫn tuyệt đối là **/ home / username**
> ## Lệnh cd
>
Để chuyển hướng trong hệ thống tập tin và thư mục Linux, bạn có thể sử dụng lệnh `cd`. Nó sẽ cần nhập đường dẫn đầy đủ hoặc tên thư mục bạn muốn chuyển tới.  
Nếu bạn đang ở trong **/home/username/Documents** và muốn đến **Photos**, thư mục con của **Documents**, chỉ cần gõ `cd Photos`.  
Trường hợp khác là nếu bạn muốn chuyển sang danh mục hoàn toàn mới, như **/home/username/Movies**. Lúc này, bạn phải gõ `cd` theo danh mục đường dẫn hoàn chỉnh như sau: `cd / home / username / Movies`.  
Có một số phím tắt giúp bạn điều hướng nhanh chóng:  

`cd ..`: để di chuyển một thư mục lên trên
`cd`: để chuyển thẳng đến thư mục chính
`cd-`: để chuyển đến thư mục trước của bạn
