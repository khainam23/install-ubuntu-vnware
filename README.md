# install-ubuntu-vnware

# Hướng dẫn cài đặt ubuntu trên máy ảo VMWare

- Nội dung của bài viết xoay quanh việc cài đặt hệ điều hành Linux cụ thể là Ubuntu tùy phiên bản bạn mong muốn, tuy nhiên trong bài viết này mình sử dụng 20.04.6 live server. Các file cài đặt link, key mình sẽ đính kèm trong bài viết nên bạn có thể thực hiện từng bước để cài đặt.

- Trước hết mình mong muốn các bạn có thể tuân thủ các quy tắc được đề ra ☑️:
    + Hãy đặt câu hỏi đúng vị trí
    + Bài viết có thể coppy nhưng hy vọng các bạn ghi nguồn 😘 

# Cài đặt VMWare 
- Các bạn tải tại [VMWare](https://devopsedu.vn/wp-content/uploads/2024/02/vmware-workstation-16.zip)
- Hoặc có thể tải tại các nguồn khác.
- Sau khi tải xong truy cập vào phần: *Help > Enter a License Key > (nhập thử các key có trong file tải)*
- Hình ảnh minh họa:
![Minh họa nhập key](image.png)

# Cài đặt Ubuntu
- Các bạn có thể chọn các phiên bản khác, ở đây mình sử dụng *Ubuntu 20.04.6 live server*.
- Và mình sử dụng file **.iso** nên có thể sẽ khác với một số bạn cài cách khác.
- Các bạn tải hệ điều hành tại link sau: [Ubuntu](https://drive.google.com/file/d/1afGhYZxcZ27dg5sZp3pkB3O4E02L6YI7/view?usp=sharing)

- Sau khi cài đặt các bạn lựa chọn mạng cấu hình cho máy ảo:
    + Bridge: Giúp các máy trong cùng mạng kết nối với nhau - Khuyến cáo cho **Máy tính bàn**
    + NAT: Máy ảo chỉ chạy trên một máy mình máy bạn - Khuyến cáo cho **Laptop**

- Chọn vào file, hoặc tại màn hình chính VMWare chọn vào thêm máy ảo:
![Chọn cài đặt máy ảo](image-1.png)

***Lưu ý:*** Các bạn nhớ giải nén toàn bộ file và đặt tại 1 thư mục cụ thể

- Sau đó các bạn có thể làm theo các bước:
## Bước 1: Nhấn "Next":
![Lựa chọn 1](image-2.png)

## Bước 2: 
+ Chọn vào mục lựa chọn *.iso*:
    ![Lựa chọn iso](image-3.png)
+ Nhấn vào "Browse", chọn tới vị trí đã đặt file ubuntu giải nén:
    ![Lựa chọn file Ubuntu đã giải nén](image-4.png)
+ Nhấn "Next"

## Bước 3: Nhập các thông tin cho người dùng máy ảo này
![Nhập thông tin](image-5.png) 

## Bước 4: Thông tin cho máy ảo
![Thông tin cho máy ảo](image-6.png)

## Bước 5: Cấu hình thông tin đĩa lưu trữ
+ Ở đây mình khuyến cáo các bạn nên để 20gb, hoặc các bạn máy yếu có thể đề từ 10gb đến 15gb 
![Cấu hình không gian đĩa](image-7.png)

## Bước 6: Kiểm tra và điều chỉnh thông tin phần cứng
+ Mặc định mạng được lựa chọn là NAT nên nếu các bạn để nguyên và nhấn "Next" thì cũng được
+ Mình sẽ hướng dẫn cấu hình chi tiết các bạn theo hướng trên có thể bỏ qua nha:
+ Các bạn nhấn vào "Customize Hardware..."
    ![Truy cập cấu hình chi tiết](image-8.png)
+ Giao diện hiện lên như sau:
    ![Giao diện cấu hình chio tiết](image-9.png)
+ Tại phần "Network Adapter" mình sẽ lựa chọn giữ nguyên *NAT*
    ![Lựa chọn mạng cấu hình](image-10.png)
+ Rồi các bạn nhấn vào phần "Close"
+ Sau đó nhấn "Finish"

## Bước 7: Cài đặt cho máy ảo
***Lưu ý:*** Sử dụng các phím *mũi tên* để lựa chọn option, sử dụng *tabs* để chọn tính năng, *enter* để nhấn đồng ý lựa chọn
    + Sau khi máy ảo được khởi động
        ![Khởi động máy ảo](image-11.png)
    + Lựa chọn ngôn ngữ, mình sử dụng "English"
        ![Lựa chọn ngôn ngữ](image-12.png)
    + Lựa chọn update, phần này thì tùy cá nhân bạn nhưng với mình thì mình sẽ lựa chọn không update, chọn "Continue without updating" và nhấn *enter*
        ![Lựa chọn update](image-13.png)
    + Tiếp đến nhấn *enter* cho tới khi gặp màn hình phía dưới
        ![Dừng lại để cài đặt thông tin](image-14.png)
    + Các bạn nhấn *phím lên* tới phần này
        ![Lựa chọn không gian](image-15.png)
    + Nhấn *enter* chọn vào *edit*
        ![Lựa chọn không gian còn trống](image-16.png)
    + Nếu lúc đầu các bạn lựa chọn ***20gb*** thì lúc này hãy nhập 18.222 còn các bạn khác có thể xem không gian còn lại và nhập nó
        ![Xem không gian còn lại](image-17.png)
    + Nhấn "Done" và chọn "Continue"
        ![Xác nhận lựa chọn](image-18.png)
    + Nhập các thông tin giống ban đầu hoặc tùy bạn custome:
        ![Nhập thông tin](image-19.png)
    + Tại mục kế tiếp bạn chọn vào "Install OpenSSH Server"
        ![Chọn cài đặt SSH](image-20.png)
    + Tiếp đó nhấn "Done" tại các màn hình khác cho tới khi gặp màn hình tải
        ![Màn hình tải](image-21.png)
    + Khi thấy màn hình hiển thị việc cancel cho update bạn nhấn vào
        ![Hủy update](image-22.png)
    + Sau đó bạn chờ cho quá trình cài đặt hoàn tất
    + Tiến hành nhập các thông tin đăng nhập
        ![Nhập thông tin đăng nhập](image-23.png)
    + Các bạn chú ý địa chỉ ip ở dòng này
        ![Địa chỉ ip](image-24.png)
    + Sử dụng Terminal trên windown, nhập lệnh sau và thay thế theo các thông tin bạn đã nhập
        ![Truy cập từ xa ubuntu bằng terminal](image-25.png)
    + Nhập "Yes" sau đó nhập mật khẩu
        ![Nhập thông tin](image-26.png)
    + Nhập lệnh `sudo -i` để truy cập vào root 
        ![Truy cập vào root](image-27.png)

## Bước 8: Sửa wifi sang tĩnh để tránh tình trạng cài đặt lại
+ Bạn mở lại VMWare vào phần **Edit > Virtual Network Editor**
+ Lựa chọn vào mục 2 vào chọn *NAT Setting*
    ![Lựa chọn xem thông tin mạng NAT](image-28.png)
+ Chú ý vào phần địa chỉ ip này
    ![Địa chỉ ip](image-29.png)
+ Mở terminal trên win, nhập lệnh chỉnh sửa
    `vi /etc/netplan/00-installer-config.yaml`
    ![Truy cập file sửa địa chỉ mạng](image-30.png)
+ Nhấn "i" và sửa thông tin tương ứng thành:
    ![Sửa thông tin](image-31.png)
+ Nhấn "esc" sau đó nhập ":x" để lưu lại và thoát
+ Sau đó nhập lệnh để áp dụng
    `netplan apply`
+ Tiến hành thử connect lại với ubuntu bằng terminal của win
    ![Thử connect lại](image-32.png)

### -- Vậy là đã kết thúc quá trình thiết lập ubuntu --    
