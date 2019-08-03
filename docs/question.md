# Unix focus question :color:

## What is difference between Unix and Linux /Solaris?
- Về cơ bản Linux và Solaris đều base trên unix.

| Unix | Linux | Solaris |
|----|-------------|-----|
|là hệ điều hành hoàn thiện được viết vào những năm 1960 và 1970 | Là một hệ điều hành mã nguồn mở dựa trên unix.Linux là tên của một kernel.|Base trên unix do Sun Microsystem phát triển|
|Trước kia phải thao tác với CLI(Command line interface). Tuy nhiên gần đây giao diện đồ họa (Graphical user interface) đã xuất hiện trên unix |Linux có cả GUI và CLI . Linux còn có 2 phần mềm cung cấp giao diện hình nền là GNOME và KDE|Giao diện dựa trên Java Desktop System (JDS) dựa trên GNOME|
|Unix không linh hoạt như linux. Muốn cài đặt unix còn tùy vào độ tương thích của phần cứng (phải nằm trong danh sách tương thích của unix)|Linux thì linh hoạt hơn có thể cài trên hầu hết các máy|Có thể cài trên hầu hêt máy|
|Unix không phải là hệ điều hành mã nguồn mở và miễn phí => Không thể custom unix theo ý mình|Linux là hệ điều hành mã nguồn mở và có thể sử dụng mã nguồn của nó miễn phí => Có thể custom linux theo ý mình|Từ 2005 - 2010 là open source. Từ 2010 - nay là close source|
|Được dùng chủ yếu cho máy server các hệ thống máy tính cao cấp tại các tổ chức lớn|Được sử dụng cho mọi đối tượng từ không chuyên -> expert|
|Hỗ trợ rất it file system: zfs, js, hfx, gps, xfs, vxfs|Hỗ trợ xfs,ramfs, nfs, vfat, cramfsm ext3, ext4, ext2,ext1, ufs, autofs, devpts, ntfs….|zfs,ufs,hsfs,pcfs,udfs|
|UNIX có rất ít phiên bản (distribution):AIS(IBM),BSD,HP-UX,Solaris|Có khá nhiều Distro của Linux đang được lưu hành:Redhat, Slackware, Debian, Solaris, Ubuntu, Centos, Fedora|OpenIndiana, illumos, Dyson|

## Which platform have you been used in last project /How many platform ?
- Gồm 2 platform hay dùng là Windows10 và Ubuntu.
## How to kill a process
- Để xóa một process ta phải biết được vị trí chính xác của process đó, và pid của chúng ta có thể sử dụng các lệnh ```top```, ```ps aux```, hoặc ta có thể filter danh sách các process bằng lệnh grep ví dụ khi ta muốn tìm process là nginx ta gõ ```ps aux | grep -i nginx```
- Hoặc khi ta đã biết chính xác tên của process ta có thể dùng ```pidof nginx``` hoặc nếu ta không nhớ rõ tên ```pgrep ngin```
- Để kill process ta gõ ```kill -9 PID``` ví dụ một process có pid là 2345 ```kill -9 2345```
## How to search multi words in a file
- Để search nhiều từ trong một file ```grep 'word1\|word2\|word3' /path/to/file```
## How to find a file having a text
- Để tìm một đoạn test xem nó có trong những file nào ta chạy lệnh ```grep -iRl "your-text-to-find" /path/to/find```
  - Trong đó -i: ignore text case
  - -R: recursively(đệ quy) tìm kiếm cả trong thư mục con
  - l: hiển thị tên file thay vì nội dung bên trong
## How to setup environment variable in Unix.
- Để set biến môi trường ta có thể sử dụng lệnh ví dụ khi set biến cho JAVA_HOME 
- ```export JAVA_HOME=/usr/java/jdk1.5.0_07/bin/java```
- ```export PATH=$PATH:/usr/java/jdk1.5.0_07/bin```
- Ta có thể set global config cho tất cả user trong file .profile hoặc bash.rc thêm đoạn export ở trên vào
```
cd
vim .bashrc
```
- Sau khi sửa xong ta dùng lệnh source .bashrc để đọc lại lệnh trong file ta mới thay đổi.
## How to install a package/a program
- Chạy lệnh ```sudo apt-get install tên_package```
## How to create a execute file.
- Để tạo một execute file ta tạo một file đuôi .sh như sau ```echo "pwd" >> test.sh```
## How to change permission /owner of a file
- Để thay đổi quyền của một file ta sử dụng lệnh chmod. Cơ bản có 3 loại user tương tác với một file như sau:
  - owner: Là người đã tạo file hoặc thư mục
  - group: Tất cả người dùng cùng thuộc 1 group
  - other: Tất cả người dùng khác
- Để muốn những user nào có quyền nào ta dùng chmod để điều khiển việc đó ví dụ: ```chmod 777 test.sh```
- 777 tượng trưng cho owner,group,other đều có cả ba quyên read,write,execute. Trong đó con số 7 là bao gồm của:
  - 4 (read) r
  - 2 (write) w
  - 1 (execute) e
- Đổi chủ sở hữu file ```chown [owner/group owner] [file name]```
## How to compare 2 text file
- Sử dụng lệnh diff để so sánh 2 file ```diff file1 file2```
- Chỉ show ra thông báo nếu 2 file khác nhau ```diff -q file1 file2```
- Chỉ show ra thông báo nếu 2 file giống nhau ```diff -s file1 file2```
