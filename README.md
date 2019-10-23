# Hướng dẫn sử dụng GIT
1. Tải git và cài đặt git về máy. Link cài đặt git https://git-scm.com/download/win
2. Tạo một tài khoản github https://github.com/
3. Tạo mới một repository.
3. Clone repository về máy. Trên màn hình làm việc của git bash gõ git clone + địa chỉ
    - Cú pháp: git clone https://github.com/hohuypn/demo.git
4. Tạo branch (Mỗi thành viên trong nhóm sẽ có một branch để làm việc, tránh bị xung đột code khi đang làm):
    - Cú pháp: git branch + tên tên nhánh
    - VD: git branch user
    Hoặc
    - git checkout -b + tên nhánh
5. push: dùng lệnh này để đẩy code lên git
    - Cú pháp: git push
6. commit: dùng lệnh commit để viết nội dung mình vừa đầy lên là phần nào trong đồ án
    - Ví dụ: git commit - m "register". Mục đích lệnh là để mô tả cho các thành viên khác biết là thành viên nào đó đang đẩy lên phần đăng ký của đồ án
    - Cú pháp: git commit -m + nội dung message. -m ở đây có nghĩa là message, cái tin nhắn mình muốn show ra cho người khác biết
7. pull: Lệnh này dùng để kéo file trên git về máy local
    - Ví dụ: kéo file register mới push lên git để làm việc
    - Cú pháp: git pull origin + tên nhánh
8. checkout: tới branch mà chúng ta làm
    - Ví dụ: Sau khi chúng ta làm xong một chức năng nào đó thì chúng ta sẽ trở về nhánh master thì chúng ta dùng lệnh này
    - Cú pháp: git checkout + tên nhánh
9. status: Lệnh này để kiểm tra trạng thái
    - Cú pháp: git status
10. merge: Nếu bạn đã chắc chắn đã làm xong phần chức năng mà bạn đảm nhiệm thì lệnh merge được dùng
    - Cú pháp: git merge + tên nhánh muốn merge
11. init: khởi tạo một việc theo dõi repository
    - Cú pháp: git init
12. git add <name> hoặc git add .
    - git add <name> là add từng file
    - git add . là add tất cả các file
13. Nếu khi add hoặc thao tác gì đó có xuất hiện kiểu như sau:
    -The file will have its original line endings in your working directory. warning: LF will be replaced by CRLF in Gemfile.
    -The file will have its original line endings in your working directory. warning: LF will be replaced by CRLF in Gemfile.lock.
    -The file will have its original line endings in your working directory. warning: LF will be replaced by CRLF in README.
 => Thì cách để không cho nó xuất hiện nữa là: git config core.autocrlf true
    
 14. Khi xuất hiện như thế này:
 
 
 ![Screenshot_1](https://user-images.githubusercontent.com/50701095/67384062-a60b6e80-f5ba-11e9-9b37-36fee904eb04.png)
 
 
 => Fix:  git config core.autocrlf true

 
 
![2019-09-13 (2)](https://user-images.githubusercontent.com/50701095/64855540-4d0afb00-d64a-11e9-94d8-8d6d2fd3cf5c.png)


Thì có thể gõ như sau:


![Screenshot_2](https://user-images.githubusercontent.com/50701095/64855634-89d6f200-d64a-11e9-9b62-29418dc7c156.png)




1. Fix lỗi khi không thể clone đồ án về local: git config --global http.proxy "192.168.101.253:3128"
2. Fix lỗi khi không thể push đồ án lên github: Khi đang ở nhánh master:
 - git pull --rebase
 - git push Khi đang ở nhánh dev
 -  git pull --rebase origin master
 - git push origin master
14. Lỗi khi add
