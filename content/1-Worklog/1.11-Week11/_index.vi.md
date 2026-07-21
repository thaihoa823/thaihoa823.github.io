---
title: "Worklog Tuần 11"
date: 2026-06-29
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---




### Mục tiêu tuần 11:

* Tìm hiểu cách xây dựng và bảo vệ API trong kiến trúc serverless trên AWS.

* Thực hành xác thực người dùng bằng Amazon Cognito và kiểm soát truy cập API.

* Làm quen với AWS WAF, AWS Lambda và S3 Presigned URL để hỗ trợ tải tệp an toàn.


### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Tìm hiểu quy trình tải tệp an toàn lên Amazon S3.<br>- Nghiên cứu cách API Gateway, Lambda và S3 phối hợp trong kiến trúc serverless.<br>- Làm quen với việc sử dụng token để xác minh yêu cầu từ người dùng. | 29/06/2026 | 29/06/2026 | <https://cloudjourney.awsstudygroup.com/vi/1.11-project-p1/><br><https://000078.awsstudygroup.com/vi/> |
| 3 | - Thực hành tạo Amazon Cognito User Pool và App Client.<br>- Thiết lập phương thức đăng nhập, chính sách mật khẩu và xác minh tài khoản.<br>- Tìm hiểu cách Cognito phát hành token sau khi người dùng đăng nhập thành công. | 30/06/2026 | 30/06/2026 | <https://cloudjourney.awsstudygroup.com/vi/1.11-project-p1/cognito/><br><https://000081.awsstudygroup.com/vi/2-create-user-pool/> |
| 4 | - Tạo các route và phương thức HTTP trong Amazon API Gateway.<br>- Tích hợp API Gateway với AWS Lambda để xử lý yêu cầu.<br>- Cấu hình Cognito Authorizer nhằm giới hạn API cho người dùng đã xác thực. | 01/07/2026 | 01/07/2026 | <https://cloudjourney.awsstudygroup.com/vi/1.11-project-p1/apigateway/><br><https://000079.awsstudygroup.com/vi/1-introduction/><br><https://000117.awsstudygroup.com/6-identity/6.8-authorizer/> |
| 5 | - Tìm hiểu cách AWS WAF bảo vệ website và API trước các yêu cầu không hợp lệ.<br>- Làm quen với Web ACL, AWS Managed Rules và cơ chế giới hạn số lượng yêu cầu.<br>- Thực hành liên kết Web ACL với tài nguyên cần bảo vệ. | 02/07/2026 | 02/07/2026 | <https://cloudjourney.awsstudygroup.com/vi/1.11-project-p1/waf/><br><https://000026.awsstudygroup.com/vi/3-useawswaf/> |
| 6 | - Xây dựng Lambda function để tạo S3 Presigned URL có thời hạn sử dụng giới hạn.<br>- Kiểm tra quyền IAM cần thiết để Lambda truy cập S3.<br>- Thử nghiệm quá trình gọi API và tải tệp lên S3 mà không cấp quyền ghi công khai cho Bucket. | 03/07/2026 | 03/07/2026 | <https://cloudjourney.awsstudygroup.com/vi/1.11-project-p1/lambda-handler/><br><https://000078.awsstudygroup.com/vi/><br><https://000033.awsstudygroup.com/vi/6-demo/> |


### Kết quả đạt được tuần 11:

* Hoàn thành cấu hình Amazon Cognito User Pool và App Client.

* Xây dựng được các route API Gateway tích hợp với AWS Lambda.

* Áp dụng Cognito Authorizer để kiểm soát quyền truy cập API.

* Thiết lập AWS WAF nhằm tăng khả năng bảo vệ API trước các yêu cầu bất thường.

* Tạo được S3 Presigned URL để hỗ trợ tải tệp an toàn trong thời gian giới hạn.

* Kiểm tra thành công luồng xác thực, gọi API và tải dữ liệu lên Amazon S3.