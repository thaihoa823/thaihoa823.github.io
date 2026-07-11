---
title: "Worklog Tuần 10"
date: 2026-06-15
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

{{% notice warning %}}
Lưu ý: Nội dung dưới đây chỉ dùng để tham khảo, vui lòng không sao chép nguyên văn cho báo cáo của bạn.
{{% /notice %}}


### Mục tiêu tuần 10:

* Tìm hiểu các khái niệm cơ bản về hybrid DNS.
* Hiểu Route 53 Resolver inbound endpoint, outbound endpoint và resolver rule.
* Thực hành kiểm tra kết nối DNS đơn giản giữa môi trường AWS và môi trường on-premises mô phỏng.


### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Tìm hiểu mục đích của Amazon Route 53 và Route 53 Resolver <br> - Hiểu ý tưởng cơ bản của hybrid DNS <br> - Tìm hiểu inbound endpoint, outbound endpoint và resolver rule | 15/06/2026 | 15/06/2026 | <https://000010.awsstudygroup.com/> |
| 3 | - Xem kiến trúc của bài thực hành <br> - Tạo hoặc kiểm tra key pair và Security Group cần thiết <br> - Triển khai các tài nguyên VPC mẫu bằng CloudFormation template | 16/06/2026 | 16/06/2026 | <https://000010.awsstudygroup.com/2-preparation/> |
| 4 | - Tìm hiểu môi trường AWS Managed Microsoft AD được dùng để mô phỏng hệ thống DNS on-premises <br> - Kiểm tra các thiết lập VPC, subnet và DNS <br> - Xác minh các tài nguyên cần thiết đã sẵn sàng | 17/06/2026 | 17/06/2026 | <https://000010.awsstudygroup.com/4-microsoft-ad-deployment/> |
| 5 | - Tạo hoặc kiểm tra Route 53 Resolver outbound endpoint <br> - Tạo resolver forwarding rule đơn giản <br> - Gắn rule vào VPC được chọn | 18/06/2026 | 18/06/2026 | <https://000010.awsstudygroup.com/5-setuphyriddns/5.1-createoe/> <br> <https://000010.awsstudygroup.com/5-setuphyriddns/5.2-createroute53/> |
| 6 | - Tạo hoặc kiểm tra Route 53 Resolver inbound endpoint <br> - Kiểm tra phân giải tên miền giữa môi trường AWS và môi trường on-premises mô phỏng <br> - Ghi lại kết quả kiểm tra <br> - Xóa các tài nguyên tạm thời sau khi thực hành | 19/06/2026 | 19/06/2026 | <https://000010.awsstudygroup.com/5-setuphyriddns/5.3-createie/> <br> <https://000010.awsstudygroup.com/5-setuphyriddns/5.4-test-results/> <br> <https://000010.awsstudygroup.com/6-clean-up-resources/> |


### Kết quả đạt được tuần 10:

* Hiểu mục đích cơ bản của hybrid DNS.

* Biết ý nghĩa cơ bản của:
  * Route 53 Resolver
  * Inbound endpoint
  * Outbound endpoint
  * Resolver rule
  * DNS forwarding

* Tìm hiểu kiến trúc kết nối DNS giữa AWS và môi trường DNS on-premises mô phỏng.

* Sử dụng CloudFormation template để tạo hoặc kiểm tra các tài nguyên mạng cần thiết.

* Kiểm tra các thiết lập VPC, subnet, Security Group và DNS.

* Hiểu cách outbound endpoint chuyển tiếp DNS query đến hệ thống DNS khác.

* Tạo hoặc kiểm tra resolver forwarding rule đơn giản.

* Gắn resolver rule vào VPC.

* Hiểu cách inbound endpoint nhận DNS query từ hệ thống DNS bên ngoài.

* Kiểm tra phân giải tên miền cơ bản giữa hai môi trường.

* Ghi lại kết quả kiểm tra DNS.

* Xóa các tài nguyên tạm thời sau khi hoàn thành thực hành.