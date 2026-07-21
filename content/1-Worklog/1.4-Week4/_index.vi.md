---
title: "Worklog Tuần 4"
date: 2026-05-11
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

### Mục tiêu tuần 4:

* Tìm hiểu các hình thức lưu trữ dữ liệu phổ biến trên AWS gồm Object Storage, Block Storage và File Storage.

* Nắm được cách bảo vệ, phân loại và tối ưu chi phí lưu trữ dữ liệu.

* Làm quen với các phương pháp sao lưu và khôi phục tài nguyên trên AWS.


### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| 2 | - Tìm hiểu Amazon S3 và các lớp lưu trữ dành cho dữ liệu có tần suất truy cập khác nhau.<br>- Làm quen với S3 Glacier dành cho dữ liệu cần lưu trữ lâu dài.<br>- Tìm hiểu Bucket Versioning, Bucket Policy và Block Public Access để bảo vệ dữ liệu. | 07/05/2026 | 07/05/2026 | <https://000057.awsstudygroup.com/vi/><br><https://000078.awsstudygroup.com/vi/> |
| 3 | - Tìm hiểu Amazon EBS và các loại ổ đĩa SSD, HDD phù hợp với từng nhu cầu sử dụng.<br>- Nghiên cứu cách tạo EBS Snapshot để sao lưu dữ liệu.<br>- Tìm hiểu quy trình khôi phục một EBS Volume từ Snapshot đã có. | 08/05/2026 | 08/05/2026 | <https://000004.awsstudygroup.com/vi/5-amazonec2basic/5.2-createec2snapshot/><br><https://100000.awsstudygroup.com/vi/1-intro/>  |
| 4 | - Phân biệt Object Storage, Block Storage và File Storage.<br>- Làm quen với Amazon EFS và Amazon FSx trong việc cung cấp hệ thống tệp dùng chung.<br>- Tìm hiểu sự khác nhau giữa EBS, EFS và S3. | 11/05/2026 | 11/05/2026 | <https://100000.awsstudygroup.com/vi/1-intro/> |
| 5 | - Tìm hiểu AWS Storage Gateway và vai trò kết nối hệ thống lưu trữ nội bộ với AWS.<br>- Làm quen với quá trình tạo File Gateway và File Share.<br>- Tìm hiểu cách dữ liệu từ môi trường nội bộ được đồng bộ lên Amazon S3. | 12/05/2026 | 12/05/2026 | <https://000024.awsstudygroup.com/vi/2-useawsstoragegw/> |
| 6 | - Tìm hiểu AWS Backup và cách quản lý hoạt động sao lưu tập trung.<br>- Làm quen với Backup Vault, Backup Plan và Recovery Point.<br>- Thực hành thiết lập kế hoạch sao lưu cho EBS và kiểm tra khả năng khôi phục dữ liệu.<br>- Xóa các tài nguyên thực hành không còn sử dụng. | 13/05/2026 | 13/05/2026 | <https://000013.awsstudygroup.com/vi/> |


### Kết quả đạt được tuần 4:

* Phân biệt được ba loại lưu trữ chính:
  * Object Storage
  * Block Storage
  * File Storage

* Hiểu Amazon S3 phù hợp với việc lưu trữ tệp, dữ liệu tĩnh và dữ liệu có dung lượng lớn.

* Biết sử dụng Versioning, Bucket Policy và Block Public Access để tăng khả năng bảo vệ dữ liệu trong S3.

* Hiểu S3 Glacier được sử dụng cho dữ liệu ít truy cập và cần lưu trữ lâu dài.

* Biết Amazon EBS cung cấp ổ đĩa khối cho EC2 và có thể sao lưu bằng Snapshot.

* Phân biệt được vai trò cơ bản của Amazon S3, Amazon EBS và Amazon EFS.

* Hiểu AWS Storage Gateway hỗ trợ kết nối hệ thống lưu trữ nội bộ với AWS Cloud.

* Làm quen với AWS Backup và các thành phần:
  * Backup Vault
  * Backup Plan
  * Recovery Point
