# Tìm hiểu, sử dụng Github  
## **1. Git và Github**
* Git : là 1 trong những hệ thống quản lý phiên bản phân tán, vốn được phát triển nhằm quản lý mã nguồn (source code) hữu hiệu của Linux.
* Github : là một website dùng để quản lý mã nguồn trực tuyến, hoạt động giống như một mạng xã hội cho lập trình viên. Dịch vụ này sử dụng Git làm nền tảng. Github chính là một dịch vụ máy chủ repository công cộng, mỗi người có thể tạo tài khoản trên đó để tạo ra các kho chứa của riêng mình để có thể làm việc.   

### **2. Các khái niệm, thao tác với github**  
### 2.1. Repository 
* là một thư viện nơi chứa các files, quản lý tất cả các thông tin cần thiết. Nơi ghi lại trạng thái của thư mục và file. 
* có 2 loại Repo: remote Repo và local repo. 
Khởi tạo repo đưa repo từ local lên github 
* Khởi tạo repo local, liên kết với tên và mail trên github, tạo thêm thư mục .git, tập tin Test.txt. 
![](https://i.imgur.com/a1k9Oni.png) 
* Đẩy repo lên repo tạo sẵn trên github 
![Imgur](https://i.imgur.com/oDkf4eL.png) 
![Imgur](https://i.imgur.com/NYjJpnk.png)  

### 2.2. Commit  
* Commit: Ghi lại trạng thái thay đổi tại máy local,bằng việc lần theo commit này từ trạng thái mới nhất thì có thể hiểu được lịch sử thay đổi trong quá khứ hoặc nội dung thay đổi đó.

### 2.3. Clone  
Clone: Để sao chép remote repository, sẽ thực hiện thao tác này Khi thực hiện Clone, sẽ tải về toàn bộ nội dung của remote repository, và có thể tạo thành local repository ở máy khác. Lịch sử thay đổi cũng được sao chép nên có thể tham chiếu lịch sử hoàn toàn giống với Repository gốc và có thể commit. 
* Tạo ra một bản sao làm việc của remote repo bằng cách chạy lệnh: `git clone <địa chỉ file trên github>`
![](https://i.imgur.com/lsO9iey.png)  
* Ta có thể thêm vào đó các chỉ số 
* Cuối cùng để lưu trữ file vừa tạo vào kho chứa Local thì ta sử dụng lệnh `git commit -m"ghi chú của việc commit"`  

### 2.4. Push
* Đẩy những thay đổi từ máy trạm lên server 
* Để chia sẻ lịch sử thay đổi của local repository mà bản thân đang có bằng remote repository, cần phải upload lịch sử thay đổi trong local repository.  Khi thực hiện Push, lịch sử thay đổi của bản thân sẽ được upload lên remote repository và lịch sử thay đổi của remote repository sẽ có trạng thái giống với local repository.
* Ta dùng lệnh `git push origin master`  

### 2.5. Pull
* Đồng bộ trạng thái từ server về máy trạm 
* Khi nhiều người chia sẻ Remote Repo và nhiều người cũng thực hiện công việc, thì mọi người sẽ push lên remote repository. Khi đó, cần lấy nội dung thay đổi mà người khác đã push lên đem vào local repository của bản thân. Thao tác này gọi là pull. 
* ta dùng `git pull origin master`
### 2.6 Branch
* Branch dùng để phân nhánh và ghi lại luồng của lịch sử. Branch đã phân nhánh sẽ không ảnh hưởng gì đến branch khác nên có thể tiến hành nhiều thay đổi đồng thời trong cùng 1 repository.
