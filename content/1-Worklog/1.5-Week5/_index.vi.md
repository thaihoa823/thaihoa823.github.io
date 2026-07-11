---
title: "Worklog Tuần 5"
date: 2026-05-11
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

{{% notice warning %}} 
⚠️ **Lưu ý:** Các thông tin dưới đây chỉ nhằm mục đích tham khảo, vui lòng **không sao chép nguyên văn** cho bài báo cáo của bạn, kể cả phần cảnh báo này.
{{% /notice %}}


### Mục tiêu tuần 5:

* Hiểu các khái niệm nền tảng và những tính năng chính của Amazon Relational Database Service (Amazon RDS).
* Biết cách tạo, cấu hình, kết nối, giám sát, sao lưu và khôi phục RDS database instance.
* Hiểu bảo mật cơ sở dữ liệu, Multi-AZ deployment, Read Replica và tính sẵn sàng cao.
* So sánh Amazon RDS với Amazon DynamoDB được sử dụng trong dự án Smart Image Platform.


### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Tìm hiểu về Amazon Relational Database Service (Amazon RDS) <br>&emsp; + Khái niệm cơ sở dữ liệu quan hệ <br>&emsp; + Các database engine được hỗ trợ <br>&emsp; + DB instance class <br>&emsp; + Các loại storage <br>&emsp; + Database endpoint <br>&emsp; + Automated backup và maintenance <br> - Tìm hiểu sự khác nhau giữa cơ sở dữ liệu tự quản lý trên EC2 và cơ sở dữ liệu được quản lý bằng Amazon RDS | 11/05/2026 | 11/05/2026 | <https://000005.awsstudygroup.com/> |
| 3 | - Chuẩn bị môi trường mạng và bảo mật cho Amazon RDS <br> - **Thực hành:** <br>&emsp; + Tạo hoặc kiểm tra VPC <br>&emsp; + Tạo public và private subnet <br>&emsp; + Tạo DB Subnet Group <br>&emsp; + Tạo Security Group cho EC2 application server <br>&emsp; + Tạo Security Group riêng cho Amazon RDS <br>&emsp; + Chỉ cho phép MySQL traffic trên port 3306 từ EC2 Security Group <br>&emsp; + Kiểm tra nguyên tắc phân quyền tối thiểu khi truy cập cơ sở dữ liệu | 12/05/2026 | 12/05/2026 | <https://000005.awsstudygroup.com/> |
| 4 | - Khởi tạo hoặc sử dụng lại Amazon Linux EC2 instance làm application server <br> - Tạo Amazon RDS MySQL database instance <br> - **Thực hành:** <br>&emsp; + Chọn MySQL database engine <br>&emsp; + Cấu hình DB instance identifier, username, password và instance class <br>&emsp; + Cấu hình storage, VPC, DB Subnet Group và Security Group <br>&emsp; + Tắt public access cho cơ sở dữ liệu <br>&emsp; + Kiểm tra RDS endpoint, port, maintenance window, log và event <br>&emsp; + Kết nối từ EC2 đến RDS database bằng database endpoint | 13/05/2026 | 13/05/2026 | <https://000005.awsstudygroup.com/> |
| 5 | - Triển khai và kiểm tra ứng dụng mẫu kết nối với Amazon RDS <br> - **Thực hành:** <br>&emsp; + Cài đặt Git và các dependency cần thiết trên EC2 <br>&emsp; + Tạo database và các bảng quan hệ bằng SQL <br>&emsp; + Cấu hình ứng dụng với RDS endpoint và database credentials <br>&emsp; + Kiểm tra các thao tác tạo, đọc, cập nhật và xóa dữ liệu <br>&emsp; + Kiểm tra lỗi kết nối cơ sở dữ liệu và Security Group rule <br> - Tìm hiểu RDS monitoring, log, automated backup, manual snapshot và point-in-time recovery | 14/05/2026 | 14/05/2026 | <https://000005.awsstudygroup.com/> |
| 6 | - Tìm hiểu tính sẵn sàng cao và khả năng mở rộng trong Amazon RDS <br>&emsp; + Multi-AZ deployment <br>&emsp; + Automatic failover <br>&emsp; + Read Replica <br>&emsp; + Backup retention <br>&emsp; + Database snapshot <br> - Phân tích lớp cơ sở dữ liệu của dự án Smart Image Platform <br>&emsp; + Kiểm tra `database-stack.ts` <br>&emsp; + Kiểm tra các bảng image metadata, quota và user profile <br>&emsp; + Kiểm tra partition key, sort key và Global Secondary Index <br>&emsp; + So sánh mô hình dữ liệu quan hệ của Amazon RDS với single-table design trong Amazon DynamoDB <br>&emsp; + So sánh khả năng mở rộng, query pattern, schema design, tính sẵn sàng và chi phí <br> - Xóa các tài nguyên RDS và EC2 không còn sử dụng sau khi thực hành để tránh phát sinh thêm chi phí | 15/05/2026 | 15/05/2026 | <https://000005.awsstudygroup.com/> <br> `infrastructure/lib/stacks/database-stack.ts` <br> `backend/api-handler/src/` |


### Kết quả đạt được tuần 5:

* Hiểu mục đích của Amazon RDS và cách dịch vụ đơn giản hóa việc quản lý cơ sở dữ liệu quan hệ trên AWS.

* Hiểu các thành phần chính của Amazon RDS, bao gồm:
  * Database engine
  * DB instance
  * DB instance class
  * Storage
  * Database endpoint
  * DB Subnet Group
  * Security Group
  * Parameter Group
  * ...

* Phân biệt được việc chạy cơ sở dữ liệu trực tiếp trên Amazon EC2 và sử dụng Amazon RDS:
  * Amazon EC2 yêu cầu tự cài đặt và bảo trì cơ sở dữ liệu
  * Amazon RDS tự động hóa backup, patching, monitoring và maintenance
  * Amazon RDS cung cấp các tùy chọn tính sẵn sàng cao được quản lý
  * ...

* Chuẩn bị được môi trường mạng cho Amazon RDS, bao gồm:
  * VPC
  * Public và private subnet
  * DB Subnet Group
  * EC2 Security Group
  * RDS Security Group
  * ...

* Cấu hình RDS Security Group chỉ cho phép kết nối cơ sở dữ liệu từ EC2 application server.

* Hiểu lý do cơ sở dữ liệu không nên được công khai trực tiếp ra Internet.

* Tạo và cấu hình thành công Amazon RDS MySQL database instance.

* Kết nối được từ Amazon EC2 instance đến RDS database bằng database endpoint.

* Tạo database và các bảng quan hệ bằng SQL.

* Triển khai và kiểm tra ứng dụng kết nối với Amazon RDS.

* Kiểm tra được các thao tác cơ sở dữ liệu cơ bản:
  * Tạo dữ liệu
  * Đọc dữ liệu
  * Cập nhật dữ liệu
  * Xóa dữ liệu
  * ...

* Biết cách kiểm tra:
  * RDS log và event
  * Cấu hình cơ sở dữ liệu
  * Thông tin maintenance
  * Cấu hình automated backup
  * Thông tin hiệu năng và kết nối
  * ...

* Hiểu automated backup, manual database snapshot và quy trình khôi phục cơ sở dữ liệu.

* Hiểu mục đích của Multi-AZ deployment:
  * Đồng bộ dữ liệu đến standby instance
  * Tăng tính sẵn sàng và khả năng chịu lỗi
  * Tự động failover khi primary database không thể hoạt động
  * ...

* Hiểu mục đích của Read Replica:
  * Sao chép dữ liệu bất đồng bộ
  * Mở rộng các workload có nhiều truy vấn đọc
  * Giảm lưu lượng đọc trên primary database
  * ...

* Phân tích được các bảng Amazon DynamoDB được sử dụng trong dự án Smart Image Platform.

* Hiểu mô hình dữ liệu DynamoDB của dự án, bao gồm:
  * Partition key
  * Sort key---
title: "Worklog Tuần 5"
date: 2026-05-11
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

{{% notice warning %}}
Lưu ý: Nội dung dưới đây chỉ dùng để tham khảo, vui lòng không sao chép nguyên văn cho báo cáo của bạn.
{{% /notice %}}


### Mục tiêu tuần 5:

* Tìm hiểu các khái niệm cơ bản về Amazon RDS.
* Hiểu database engine, DB instance, subnet group và các thiết lập bảo mật.
* Thực hành tạo, kết nối và xóa một cơ sở dữ liệu RDS đơn giản.


### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Tìm hiểu mục đích của Amazon RDS <br> - Xem một số database engine được hỗ trợ như MySQL và PostgreSQL <br> - Phân biệt cơ bản giữa cơ sở dữ liệu tự quản lý và cơ sở dữ liệu được AWS quản lý | 11/05/2026 | 11/05/2026 | <https://000005.awsstudygroup.com/> |
| 3 | - Kiểm tra VPC và subnet dùng cho cơ sở dữ liệu <br> - Tạo DB subnet group <br> - Tạo Security Group cho cơ sở dữ liệu RDS | 12/05/2026 | 12/05/2026 | <https://000005.awsstudygroup.com/2-prerequisite-steps/> |
| 4 | - Tạo một cơ sở dữ liệu MySQL RDS nhỏ để thực hành <br> - Cấu hình database name, username, password, storage và connectivity <br> - Chờ trạng thái cơ sở dữ liệu chuyển sang Available | 13/05/2026 | 13/05/2026 | <https://000005.awsstudygroup.com/4-create-rds-database-instance/> |
| 5 | - Kiểm tra endpoint và port của RDS <br> - Kết nối đến cơ sở dữ liệu từ EC2 instance hoặc database client <br> - Tạo bảng đơn giản và thêm dữ liệu thử nghiệm | 14/05/2026 | 14/05/2026 | <https://000005.awsstudygroup.com/5-application-deployment/> |
| 6 | - Kiểm tra các thiết lập giám sát và sao lưu cơ bản của RDS <br> - Tạo manual snapshot để thực hành <br> - Xóa cơ sở dữ liệu, snapshot và các tài nguyên liên quan sau khi hoàn thành | 15/05/2026 | 15/05/2026 | <https://000005.awsstudygroup.com/6-backup-and-restore/> <br> <https://000005.awsstudygroup.com/7-clean-up-resources/> |


### Kết quả đạt được tuần 5:

* Hiểu mục đích cơ bản của Amazon RDS.

* Biết ý nghĩa cơ bản của:
  * Database engine
  * DB instance
  * DB subnet group
  * Database endpoint
  * Security Group
  * Snapshot

* Tìm hiểu một số database engine được Amazon RDS hỗ trợ.

* Tạo DB subnet group và Security Group cơ bản.

* Tạo một cơ sở dữ liệu MySQL RDS nhỏ để thực hành.

* Kiểm tra trạng thái, endpoint và port của cơ sở dữ liệu.

* Kết nối đến RDS từ EC2 instance hoặc database client.

* Tạo bảng đơn giản và thêm dữ liệu thử nghiệm.

* Kiểm tra các thiết lập giám sát và sao lưu cơ bản.

* Tạo manual snapshot để thực hành.

* Xóa cơ sở dữ liệu và các tài nguyên tạm thời sau khi hoàn thành.
  * Image metadata record
  * User quota record
  * User profile record
  * Global Secondary Index
  * ...

* So sánh được Amazon RDS với Amazon DynamoDB:
  * Amazon RDS sử dụng bảng quan hệ và SQL
  * DynamoDB là cơ sở dữ liệu NoSQL được thiết kế theo các query pattern xác định trước
  * Amazon RDS hỗ trợ join và các truy vấn quan hệ phức tạp
  * DynamoDB cung cấp khả năng mở rộng serverless và truy cập dữ liệu độ trễ thấp theo key
  * Smart Image Platform sử dụng DynamoDB vì metadata và luồng xử lý theo sự kiện phù hợp với kiến trúc serverless
  * ...

* Biết cách tạo final snapshot khi cần thiết và xóa các tài nguyên RDS, EC2 không còn sử dụng để giảm chi phí AWS.