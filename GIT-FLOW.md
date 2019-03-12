## EGD-Group Git flow

Flow tham khảo: [A successful Git branching model](http://nvie.com/posts/a-successful-git-branching-model/)

### Giả định
* Đã tạo Central Repository (Nguồn trung tâm) trên Github（hoặc Bitbucket）.
* Branch mặc định của Central Repository là master.
* Lập trình viên có thể  fork (tạo nhánh) đối với Central Repository.

### Tạo branch khi xử lý task
* Tất cả các branch đều phải được tách từ master.
* Nếu là chức năng mới thì branch phải có dạng: feature/task_TicketID_TicketTitle (các chữ cái của title phân cách nhau bằng dấu `_`).
* Nếu là xử lý bug thì branch phải có dạng: hotfix/task_TicketID_TicketTitle (các chữ cái của title phân cách nhau bằng dấu `_`).
* Tạo branch release phải có dạng: release/ddmmYYYY.
* Mỗi một task tương ứng với 1 branch, không được xử lý nhiều task trong cùng 1 branch.
* Tại môi trường local(trên máy dev), tuyệt đối không được thay đổi code khi ở branch master.Nhất định phải thao tác trên branch khởi tạo để làm task.

### Quy định khi commit, push
* Ngoài ra thì với gitflow trước đây ( trước thời điểm 2018/03/28) thì có cho phép dùng force push, tuy nhiên do khi sử dụng force push sẽ xoá hết lịch sử thay đổi do vậy gitlow hiện tại không khuyến khích sử dụng force push. Trong trường hợp cần sử dụng force push thì cần có sự đồng thuận từ team.
* Khi commit phải comment rõ ràng nội dung mà mình đã code, message commit phải có ít nhất 8 chữ.
  * Ví dụ
    * `Tạo method thực hiện việc clear cache trong Model`
	* `Tại controller gọi method ở Model để thực hiện việc clear cache`


