---
title: "Worklog Tuần 3"
date: 2026-04-27
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

{{% notice warning %}}
Lưu ý: Nội dung dưới đây chỉ dùng để tham khảo, vui lòng không sao chép nguyên văn cho báo cáo của bạn.
{{% /notice %}}


### Mục tiêu tuần 3:

* Tìm hiểu các khái niệm cơ bản về Amazon VPC.
* Hiểu subnet, route table, Internet Gateway và Security Group.
* Thực hành tạo môi trường mạng đơn giản và kiểm tra kết nối EC2.


### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Tìm hiểu mục đích của Amazon VPC <br> - Tìm hiểu CIDR block, public subnet và private subnet <br> - Xem các thành phần cơ bản trong một VPC | 27/04/2026 | 27/04/2026 | <https://000003.awsstudygroup.com/> |
| 3 | - Tạo một Amazon VPC đơn giản <br> - Tạo một public subnet và một private subnet <br> - Kiểm tra sơ đồ tài nguyên VPC | 28/04/2026 | 28/04/2026 | <https://000003.awsstudygroup.com/3-preparation-steps/> |
| 4 | - Tạo và gắn Internet Gateway vào VPC <br> - Tạo route table cho public subnet <br> - Thêm route kết nối đến Internet Gateway | 29/04/2026 | 29/04/2026 | <https://000003.awsstudygroup.com/3-preparation-steps/> |
| 5 | - Tạo Security Group cơ bản <br> - Chỉ cho phép SSH từ địa chỉ IP tin cậy <br> - Tìm hiểu sự khác nhau giữa Security Group và Network ACL | 30/04/2026 | 30/04/2026 | <https://000003.awsstudygroup.com/2-firewall-in-vpc/> |
| 6 | - Khởi tạo một EC2 instance nhỏ trong public subnet <br> - Kiểm tra thông tin mạng của instance <br> - Thử kết nối đến instance <br> - Xóa EC2 instance và các tài nguyên VPC tạm thời sau khi thực hành | 01/05/2026 | 01/05/2026 | <https://000003.awsstudygroup.com/4-deploy-ec2/> <br> <https://000003.awsstudygroup.com/6-clean-up-resources/> |


### Kết quả đạt được tuần 3:

* Hiểu mục đích cơ bản của Amazon VPC.

* Biết ý nghĩa cơ bản của:
  * CIDR block
  * Public subnet
  * Private subnet
  * Route table
  * Internet Gateway
  * Security Group

* Tạo được một VPC đơn giản với public subnet và private subnet.

* Tạo và gắn Internet Gateway vào VPC.

* Cấu hình route table cho public subnet.

* Tạo Security Group cơ bản cho EC2 instance.

* Hiểu sự khác nhau cơ bản giữa Security Group và Network ACL.

* Khởi tạo một EC2 instance trong public subnet.

* Kiểm tra thông tin mạng và thử kết nối đến EC2 instance.

* Xóa các tài nguyên tạm thời sau khi hoàn thành thực hành.