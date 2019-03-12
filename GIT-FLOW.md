## EGD-Group Git flow

Flow tham khảo: [A successful Git branching model](http://nvie.com/posts/a-successful-git-branching-model/)

### Giả định
* Đã tạo Central Repository (Nguồn trung tâm) trên Github（hoặc Bitbucket）.
* Branch mặc định của Central Repository là master.
* Lập trình viên có thể  fork (tạo nhánh) đối với Central Repository.
### Tạo branch khi xử lý ticket
* Tất cả các branch đều phải được tách từ master.
* Nếu là chức năng mới thì branch phải có dạng: feature/task_TicketID_TicketTitle (các chữ cái của title phân cách nhau bằng dấu `_`).
* Nếu là xử lý bug thì branch phải có dạng: hotfix/task_TicketID_TicketTitle (các chữ cái của title phân cách nhau bằng dấu `_`).
* Mỗi một ticket là 1 branch, không được xử lý nhiều task trong cùng 1 branch.

