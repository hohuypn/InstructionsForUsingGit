# Hướng dẫn sử dụng GIT
1. Tải git và cài đặt git bash về máy. Link cài đặt git bash https://git-scm.com/download/win
2. Tạo một tài khoản github https://github.com/
3. Tạo mới một repository.
3. Clone repository về máy. Trên màn hình làm việc của git bash gõ git clone + địa chỉ
    - Cú pháp: git clone https://github.com/hohuypn/demo.git
4. Tạo branch (Mỗi thành viên trong nhóm sẽ có một branch để làm việc, tránh bị xung đột code khi đang làm):
    - Cú pháp: git branch + tên branch
    - VD: git branch user
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
