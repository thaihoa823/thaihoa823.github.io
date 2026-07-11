---
title: "Worklog Tuần 6"
date: 2026-05-18
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

{{% notice warning %}}
Lưu ý: Nội dung dưới đây chỉ dùng để tham khảo, vui lòng không sao chép nguyên văn cho báo cáo của bạn.
{{% /notice %}}


### Mục tiêu tuần 6:

* Tìm hiểu các khái niệm cơ bản về Elastic Load Balancing và EC2 Auto Scaling.
* Hiểu Launch Template, Target Group và Application Load Balancer.
* Thực hành tạo một môi trường web server có khả năng mở rộng đơn giản.


### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Tìm hiểu mục đích của Elastic Load Balancing và EC2 Auto Scaling <br> - Tìm hiểu vai trò cơ bản của Load Balancer, Target Group, Launch Template và Auto Scaling Group | 18/05/2026 | 18/05/2026 | <https://000006.awsstudygroup.com/> |
| 3 | - Tạo Launch Template cho một Amazon Linux EC2 instance nhỏ <br> - Thêm user data script đơn giản để cài đặt web server <br> - Chọn Security Group và key pair cần thiết | 19/05/2026 | 19/05/2026 | <https://000006.awsstudygroup.com/2-create-launch-template/> |
| 4 | - Tạo Target Group cho các EC2 instance <br> - Cấu hình health check cơ bản <br> - Tạo Application Load Balancer trong public subnet <br> - Kết nối listener của Load Balancer với Target Group | 20/05/2026 | 20/05/2026 | <https://000006.awsstudygroup.com/3-create-target-group/> <br> <https://000006.awsstudygroup.com/4-create-load-balancer/> |
| 5 | - Tạo Auto Scaling Group bằng Launch Template <br> - Thiết lập số lượng instance tối thiểu, mong muốn và tối đa <br> - Gắn Auto Scaling Group với Target Group <br> - Kiểm tra trạng thái của các EC2 instance | 21/05/2026 | 21/05/2026 | <https://000006.awsstudygroup.com/5-create-auto-scaling-group/> |
| 6 | - Mở DNS name của Load Balancer và kiểm tra trang web <br> - Xem các CloudWatch metric cơ bản của Auto Scaling Group <br> - Thay đổi desired capacity và quan sát số lượng instance <br> - Xóa Auto Scaling Group, Load Balancer, Target Group và Launch Template sau khi thực hành | 22/05/2026 | 22/05/2026 | <https://000006.awsstudygroup.com/6-test-auto-scaling/> <br> <https://000006.awsstudygroup.com/7-clean-up/> |


### Kết quả đạt được tuần 6:

* Hiểu mục đích cơ bản của Elastic Load Balancing và EC2 Auto Scaling.

* Biết ý nghĩa cơ bản của:
  * Launch Template
  * Target Group
  * Health Check
  * Application Load Balancer
  * Auto Scaling Group

* Tạo Launch Template cho Amazon Linux EC2 instance.

* Sử dụng user data script đơn giản để cài đặt web server.

* Tạo Target Group và cấu hình health check cơ bản.

* Tạo Application Load Balancer và kết nối với Target Group.

* Tạo Auto Scaling Group với các thiết lập minimum, desired và maximum capacity.

* Kiểm tra trạng thái của EC2 instance trong Target Group.

* Truy cập trang web thử nghiệm thông qua DNS name của Load Balancer.

* Thay đổi desired capacity và quan sát số lượng EC2 instance.

* Xóa các tài nguyên mở rộng và cân bằng tải tạm thời sau khi hoàn thành thực hành.