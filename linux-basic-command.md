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

* `cd ..`: để di chuyển đến một thư mục trên  
* `cd`: để chuyển thẳng đến thư mục chính  
* `cd-`: để chuyển đến thư mục trước đó của bạn  

> ## Lệnh ls
> 
Được dùng để xem nội dung thư mục.  

Nếu muốn xem thư mục khác, hãy nhập lệnh `ls` và sau đó là đường dẫn thư mục.  

Có nhiều phiên bản để sử dụng với lệnh `ls` như sau:  

* `ls -R`: liệt kê các file bao gồm cả các thư mục phụ bên trong  
* `ls -a`: liệt kê những file ẩn  
* `ls -al`: liệt kê tất cả file và thư mục với thông tin chi tiết như phân quyền, kích thước, chủ sở hữu,...  

> ## Lệnh Cat
> 
Dùng để xem nội dung file trên output tiêu chuẩn (sdout). Để chạy lệnh này, gõ cat theo sau là tên file và phần mở rộng. Ví dụ: `cat file.txt`.  

Có nhiều cách để sử dụng cat command trong linux:  

* `cat>filename`: tạo ra file mới  
* `cat filename1 filename2>filename3`: nhập 2 files 1 và 2 để lưu kết quả vào file 3  
* `cat filename | tr a-z A-Z >output.txt`: để chuyển một file từ in thường tới in hoa hoặc ngược lại  

> ## Lệnh cp
>
Sử dụng `cp` để sao chép files từ thư mục hiện tại.  

Ví dụ: **cp scenery.jpg /home/username/Pictures** sẽ tạo bản copy của **scenery.jpg** vào danh mục **Pictures**.  

> ## Lệnh mv
> 
Công dụng chính của `mv` là di chuyển files.  

Bạn cần nhập `mv`, tên file và điểm đến của thư mục. Ví dụ: **mv file.txt /home/username/Documents**.  

Để đổi tên files, cú pháp là **mv oldname.ext newname.ext**.  

> ## Lệnh mkdir
> 
Dùng để tạo thư mục mới – giống như `mkdir Music` sẽ tạo thư mục mới gọi là **Music**.  

Để tạo một thư mục mới bên trong thư mục khác, sử dụng lệnh sau: **mkdir Music/Newfile**.  

Sử dụng p (parents) option để tạo thư mục giữa 2 thư mục đã tồn tại. Ví dụ, **mkdir -p Music/2020/Newfile** sẽ tạo thư mục “2020”.  

> ## Lệnh rmdir
> 
Nếu bạn cần xóa thư mục, sử dụng `rmdir`. Tuy nhiên, `rmdir` chỉ cho phép bạn xóa các thư mục trống.  

> ## Lệnh rm
> 
Sử dụng để xóa thư mục và nội dung bên trong. Nếu bạn chỉ muốn xóa thư mục – tương tự như lệnh `rmdir` – sử dụng `rm -r`.  

Lưu ý: Lệnh này sẽ xóa mọi thứ và không khôi phục được thư mục đó.  

> ## Lệnh touch
> 
Lệnh này cho phép bạn tạo files mới trống thông qua dòng lệnh. Ví dụ: **touch /home/username/Documents/Web.html** để tạo file *HTML* tiêu đề *Web* trong thư mục **Documents**.  

> ## Lệnh find
> 
Lệnh find dùng tìm files. Bạn sử dụng command find để xác định vị trí files trong thư mục nhất định.  

Ví dụ: **find /home/ -name notes.txt** sẽ tìm file tên notes.txt trong thư mục chính và thư mục con của nó.  

Để tìm file trong thư mục hiện tại, dùng lệnh **find . -name notes.txt**.  
Để tìm thư mục được dùng, **/ -type d -name notes. txt**.  

> ## Lệnh sudo
> 
Command sudo là viết tắt của “SuperUser Do”, cho phép bạn thực hiện các tác vụ yêu cầu quyền quản trị hoặc quyền root.  





