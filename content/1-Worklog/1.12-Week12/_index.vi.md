---
title: "Worklog Tuần 12"
date: 2026-07-06
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---



### Mục tiêu tuần 12:

* Hoàn thiện quy trình xử lý hình ảnh bất đồng bộ theo kiến trúc hướng sự kiện trên AWS.

* Tích hợp Amazon S3, AWS Lambda, DynamoDB Streams và Amazon Rekognition để tự động xử lý, phân tích và lưu trữ thông tin hình ảnh.

* Kiểm thử toàn bộ luồng hoạt động, theo dõi nhật ký và dọn dẹp các tài nguyên thực hành.


### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Tạo hai Amazon S3 Bucket riêng biệt để lưu ảnh gốc và ảnh đã xử lý.<br>- Cấu hình sự kiện Object Created để tự động kích hoạt AWS Lambda khi có ảnh mới được tải lên.<br>- Thiết lập IAM Role và quyền truy cập cần thiết cho Lambda. | 06/07/2026 | 06/07/2026 | <https://000078.awsstudygroup.com/vi/><br><https://000078.awsstudygroup.com/vi/2-resize-image-function/> |
| 3 | - Xây dựng Lambda function để đọc ảnh từ S3, thay đổi kích thước và tối ưu dung lượng ảnh.<br>- Lưu ảnh sau xử lý vào Bucket đích.<br>- Theo dõi quá trình thực thi và kiểm tra lỗi thông qua Amazon CloudWatch Logs. | 07/07/2026 | 07/07/2026 | <https://000078.awsstudygroup.com/vi/2-resize-image-function/><br><https://000008.awsstudygroup.com/vi/> |
| 4 | - Tạo bảng Amazon DynamoDB để lưu trữ metadata của hình ảnh.<br>- Xác định Partition Key và các thuộc tính cần thiết cho mỗi bản ghi.<br>- Kích hoạt DynamoDB Streams và liên kết Stream với Lambda function để xử lý các thay đổi dữ liệu. | 08/07/2026 | 08/07/2026 | <https://000078.awsstudygroup.com/vi/><br><https://000039.awsstudygroup.com/3-ladv/3.9/> |
| 5 | - Xây dựng Lambda function nhận sự kiện từ DynamoDB Streams.<br>- Tích hợp Amazon Rekognition để nhận diện vật thể, phân loại nhãn và kiểm tra nội dung hình ảnh.<br>- Cập nhật kết quả phân tích vào bảng DynamoDB. | 09/07/2026 | 09/07/2026 | <https://000056.awsstudygroup.com/vi/2-adding-object-recognition-using-aws-rekognition/><br><https://000039.awsstudygroup.com/3-ladv/3.9/> |
| 6 | - Kiểm thử toàn bộ luồng từ tải ảnh, xử lý ảnh, phân tích bằng Rekognition đến cập nhật metadata.<br>- Kiểm tra ảnh trong các S3 Bucket, dữ liệu trong DynamoDB và nhật ký thực thi trong CloudWatch.<br>- Sắp xếp mã nguồn, hoàn thiện tài liệu hướng dẫn và dọn dẹp các tài nguyên không còn sử dụng. | 10/07/2026 | 10/07/2026 | <https://000078.awsstudygroup.com/vi/4-cleanup/><br><https://000008.awsstudygroup.com/vi/><br><https://000056.awsstudygroup.com/vi/> |


### Kết quả đạt được tuần 12:

* Hoàn thành quy trình xử lý hình ảnh bất đồng bộ theo kiến trúc hướng sự kiện.

* Kết nối thành công Amazon S3 với AWS Lambda để tự động thay đổi kích thước và tối ưu hình ảnh.

* Sử dụng DynamoDB Streams để kích hoạt quá trình phân tích dữ liệu khi metadata thay đổi.

* Tích hợp Amazon Rekognition để nhận diện vật thể, gán nhãn và kiểm tra nội dung hình ảnh.

* Kiểm tra thành công toàn bộ luồng xử lý thông qua Amazon CloudWatch Logs.

* Đóng gói dự án và đẩy thành công Repo mã nguồn hoàn chỉnh có kèm file hướng dẫn cài đặt (README.md) chi tiết lên GitHub cá nhân. 