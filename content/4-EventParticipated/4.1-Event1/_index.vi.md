---
title: "Sự kiện 1"
date: 2026-06-06
weight: 1
chapter: false
pre: " <b> 4.1. </b> "
---

{{% notice warning %}}
Lưu ý: Nội dung dưới đây chỉ dùng để tham khảo, vui lòng không sao chép nguyên văn vào báo cáo của bạn.
{{% /notice %}}

# Báo cáo tổng kết: “AWS Study Group Meetup – Công nghệ, Điện toán đám mây, An ninh mạng, Trí tuệ nhân tạo và Phát triển nghề nghiệp”

### Mục tiêu sự kiện

- Giới thiệu các công nghệ thực tế được sử dụng trong phát triển phần mềm hiện đại và điện toán đám mây.
- Chia sẻ kiến thức về Docker, bảo mật AWS, hệ thống multiplayer sử dụng WebSocket, kỹ năng làm việc nhóm, GraphRAG và phát triển nghề nghiệp.
- Giúp người tham dự hiểu cách áp dụng các dịch vụ AWS vào dự án thực tế.
- Cung cấp định hướng học tập cho sinh viên quan tâm đến Cloud, DevOps, Cybersecurity, Artificial Intelligence và System Administration.
- Tạo cơ hội để người tham dự học hỏi từ các diễn giả có nền tảng kỹ thuật khác nhau.

### Diễn giả

- **Bao Huynh** – Diễn giả của chủ đề Docker và công nghệ container
- **Lê Hoàng Gia Đại** – Diễn giả của chủ đề hệ thống phát hiện xâm nhập mạng sử dụng Machine Learning trên AWS
- **Nguyễn Quốc Bảo** – Diễn giả của chủ đề game multiplayer với Godot và AWS WebSocket
- **Trương Huy Phước** – Diễn giả của chủ đề kỹ năng làm việc nhóm hiệu quả
- **Việt Phát** – Diễn giả của chủ đề GraphRAG với Amazon Bedrock và Amazon Neptune
- **Trần Trung Vinh** – System Administrator tại Central Retail Group và diễn giả của chủ đề hành trình từ IT Helpdesk đến Senior Sysadmin

### Nội dung nổi bật

#### Docker – Công nghệ đóng gói ứng dụng bằng container

Phiên trình bày đầu tiên giới thiệu Docker và vai trò của containerization trong quá trình phát triển ứng dụng hiện đại.

- Máy ảo cung cấp một môi trường hệ điều hành hoàn chỉnh, trong khi container dùng chung hệ điều hành của máy chủ và thường nhẹ hơn.
- Docker image là mẫu có thể tái sử dụng, chứa mã nguồn ứng dụng, thư viện và các dependency.
- Docker container là phiên bản đang chạy được tạo ra từ Docker image.
- Dockerfile mô tả các bước cần thiết để xây dựng image.
- Image layer cho phép Docker tái sử dụng các phần không thay đổi và tăng tốc quá trình build.
- Docker giúp các nhóm duy trì môi trường phát triển, kiểm thử và triển khai nhất quán.
- Các trường hợp sử dụng phổ biến gồm microservices, CI/CD pipeline, kiểm thử ứng dụng và triển khai trên nền tảng đám mây.

Phiên này giúp tôi hiểu vì sao container được sử dụng rộng rãi trong các hệ thống cloud-native và cách Docker giảm sự khác biệt giữa môi trường phát triển và môi trường production.

#### Hệ thống phát hiện xâm nhập mạng sử dụng Machine Learning trên AWS

Phiên trình bày thứ hai tập trung vào việc cải thiện an ninh mạng bằng cách kết hợp các dịch vụ AWS với Machine Learning.

- AWS WAF có thể bảo vệ ứng dụng web và API trước các mối đe dọa phổ biến như SQL Injection, Cross-Site Scripting, bot và brute-force.
- Hệ thống dựa trên rule có hiệu quả nhưng có thể gặp khó khăn trong việc phát hiện các kiểu tấn công mới hoặc hành vi bất thường.
- Hệ thống Network Intrusion Detection sử dụng Machine Learning có thể phân tích lưu lượng và nhận diện hành vi bất thường.
- Bộ dữ liệu CSE-CIC-IDS2018 được giới thiệu như một nguồn dữ liệu gồm lưu lượng mạng bình thường và độc hại.
- Các bước xử lý dữ liệu quan trọng gồm làm sạch dữ liệu, chọn đặc trưng phù hợp, xử lý giá trị thiếu và giải quyết tình trạng mất cân bằng dữ liệu.
- LightGBM được giới thiệu như một mô hình có thể sử dụng để phân loại lưu lượng mạng.
- Các chỉ số như accuracy, precision, recall, F1-score và confusion matrix rất quan trọng khi đánh giá mô hình bảo mật.
- Các dịch vụ AWS có thể hỗ trợ lưu trữ dữ liệu, xử lý, triển khai mô hình, ghi log và giám sát.

Chủ đề này đặc biệt phù hợp với ngành An ninh mạng của tôi vì cho thấy các biện pháp bảo mật truyền thống và Machine Learning có thể bổ trợ cho nhau.

#### Multiplayer trên nền tảng đám mây – Kết nối Godot Client bằng AWS WebSocket

Phiên trình bày thứ ba giới thiệu một kiến trúc serverless để kết nối các Godot game client thông qua AWS WebSocket.

- UDP và ENet phù hợp với gameplay thời gian thực có yêu cầu tốc độ cao, nhưng có thể cần quản lý hạ tầng phức tạp hơn.
- WebSocket cung cấp kết nối hai chiều liên tục giữa client và server.
- WebSocket phù hợp với hệ thống chat, game lobby, game theo lượt, cập nhật trạng thái và thông báo.
- Amazon API Gateway WebSocket có thể quản lý các kết nối client.
- AWS Lambda có thể xử lý các sự kiện kết nối, ngắt kết nối và gửi tin nhắn.
- Amazon DynamoDB có thể lưu connection ID và thông tin trạng thái đơn giản của người chơi.
- Amazon CloudWatch có thể lưu log và hỗ trợ xử lý sự cố.
- Kiến trúc cần xử lý các vấn đề như stale connection, tính stateless của Lambda, chi phí scan bảng và client bị ngắt kết nối.

Phiên này giúp tôi hiểu cách kết hợp các dịch vụ serverless của AWS để xây dựng một ứng dụng thời gian thực đơn giản mà không cần duy trì server truyền thống.

#### Nghệ thuật làm việc nhóm hiệu quả

Phiên trình bày thứ tư tập trung vào các yếu tố con người và tổ chức ảnh hưởng đến sự thành công của dự án.

Diễn giả trình bày bốn nguyên tắc quan trọng:

- **Mục tiêu rõ ràng và thống nhất:** Các thành viên phải hiểu kết quả cần đạt được và cùng hướng đến một mục tiêu chung.
- **Đúng người, đúng vị trí:** Công việc nên được phân chia dựa trên điểm mạnh và kinh nghiệm của từng thành viên.
- **Giao tiếp cởi mở và lắng nghe chủ động:** Các thành viên nên trao đổi trung thực, lắng nghe cẩn thận và đưa ra phản hồi mang tính xây dựng.
- **Trách nhiệm cá nhân:** Mỗi thành viên cần chịu trách nhiệm đối với nhiệm vụ và thời hạn đã được giao.

Phiên này cũng giới thiệu các công cụ hỗ trợ cộng tác như Trello, ClickUp, Google Workspace, Slack và Discord.

Bài học chính là công cụ có thể hỗ trợ làm việc nhóm nhưng không thể thay thế giao tiếp rõ ràng, tinh thần trách nhiệm và sự tôn trọng lẫn nhau.

#### Xây dựng ứng dụng GraphRAG bằng Amazon Bedrock và Amazon Neptune

Phiên trình bày thứ năm giới thiệu Retrieval-Augmented Generation và GraphRAG.

- RAG truyền thống truy xuất nội dung liên quan và cung cấp cho Large Language Model trước khi tạo câu trả lời.
- RAG truyền thống có thể gặp khó khăn khi xử lý câu hỏi cần suy luận qua nhiều thực thể có liên kết.
- GraphRAG biểu diễn tri thức bằng node, edge và relationship.
- Graph traversal có thể hỗ trợ multi-hop reasoning và tăng khả năng hiểu các mối quan hệ.
- Amazon Bedrock Knowledge Bases hỗ trợ xử lý tài liệu, chunking, embedding và retrieval.
- Amazon Neptune có thể lưu trữ và xử lý dữ liệu dạng graph.
- Cypher query có thể được sử dụng để tìm kiếm các mối quan hệ trong knowledge graph.
- Hai hướng triển khai được giới thiệu:
  - Hướng managed sử dụng Amazon Bedrock Knowledge Bases và Neptune Analytics
  - Hướng tùy chỉnh sử dụng LlamaIndex và Amazon Neptune

Phiên này giúp tôi hiểu GraphRAG hữu ích trong các trường hợp mối quan hệ giữa các thông tin quan trọng không kém bản thân thông tin.

#### Từ IT Helpdesk đến Senior Sysadmin

Phiên cuối cùng tập trung vào quá trình phát triển nghề nghiệp từ IT Helpdesk lên System Administrator, sau đó chuyển dần sang Cloud hoặc DevOps.

- IT Helpdesk giúp phát triển kỹ năng troubleshooting, giao tiếp, hỗ trợ người dùng và giải quyết vấn đề.
- Linux và networking là nền tảng quan trọng đối với System Administration.
- Xây dựng phòng lab cá nhân là cách hiệu quả để thực hành kỹ năng server, network và security.
- Công việc của System Administrator có thể gồm:
  - Quản lý server và network
  - Cập nhật bản vá bảo mật
  - Monitoring
  - Capacity planning
  - Viết tài liệu và runbook
  - Tự động hóa các công việc lặp lại
- Lộ trình học Cloud và DevOps có thể bao gồm AWS, Terraform, Docker, Infrastructure as Code và CI/CD.
- Các dự án thực tế và portfolio tốt có giá trị khi ứng tuyển vào các vị trí kỹ thuật.
- Người học nên tập trung sâu vào một số kỹ năng cốt lõi thay vì học quá nhiều công cụ nhưng không đủ thực hành.

Phiên này cung cấp một lộ trình nghề nghiệp thực tế và cho thấy kinh nghiệm Helpdesk có thể trở thành nền tảng cho các vị trí hạ tầng nâng cao hơn.

### Bài học chính

#### Kiến thức kỹ thuật

- Docker giúp đóng gói ứng dụng và dependency thành môi trường nhất quán, dễ di chuyển.
- Hệ thống bảo mật có thể kết hợp rule-based protection với Machine Learning-based anomaly detection.
- Các dịch vụ serverless của AWS có thể hỗ trợ ứng dụng thời gian thực thông qua API Gateway, Lambda, DynamoDB và CloudWatch.
- GraphRAG có thể cải thiện khả năng truy xuất thông tin khi câu hỏi phụ thuộc vào mối quan hệ giữa các thực thể.
- Linux, networking, automation và cloud là những nền tảng quan trọng cho nghề nghiệp liên quan đến hạ tầng.

#### Kiến trúc và dịch vụ đám mây

- Mỗi dịch vụ AWS nên được lựa chọn dựa trên bài toán cụ thể cần giải quyết.
- Serverless giúp giảm công việc quản lý hạ tầng nhưng vẫn cần thiết kế và giám sát cẩn thận.
- CloudWatch rất quan trọng trong việc theo dõi hoạt động hệ thống và xử lý lỗi.
- DynamoDB phù hợp để lưu trạng thái và thông tin kết nối đơn giản, nhưng nên hạn chế các thao tác scan không hiệu quả.
- Mô hình bảo mật nên được đánh giá bằng nhiều chỉ số phù hợp thay vì chỉ sử dụng accuracy.

#### Làm việc nhóm và phát triển nghề nghiệp

- Mục tiêu rõ ràng và trách nhiệm cá nhân giúp cải thiện hiệu quả làm việc nhóm.
- Công cụ kỹ thuật chỉ phát huy hiệu quả khi nhóm giao tiếp cởi mở.
- Xây dựng dự án và phòng lab cá nhân là cách hiệu quả để tăng kỹ năng thực tế.
- Một lộ trình nghề nghiệp tốt nên bắt đầu bằng nền tảng vững chắc trước khi học các công cụ nâng cao.
- Việc học liên tục là cần thiết vì công nghệ cloud, security và AI thay đổi nhanh chóng.

### Áp dụng vào học tập và công việc

Sau sự kiện, tôi xác định một số cách thực tế để áp dụng kiến thức vào việc học và các dự án:

- Sử dụng Docker để tạo môi trường nhất quán cho các dự án backend và cloud.
- Thực hành viết Dockerfile đơn giản và chạy ứng dụng trong container.
- Tìm hiểu bộ dữ liệu an ninh mạng và các kỹ thuật xử lý dữ liệu cơ bản bằng Python.
- So sánh phương pháp phát hiện dựa trên rule với phát hiện bất thường bằng Machine Learning.
- Sử dụng Amazon CloudWatch để xem log, metric và lỗi trong các dự án AWS.
- Tìm hiểu API Gateway WebSocket và Lambda cho chức năng chat, notification hoặc cập nhật trạng thái thời gian thực.
- Sử dụng DynamoDB cẩn thận để lưu thông tin kết nối hoặc session đơn giản.
- Áp dụng cách phân chia nhiệm vụ rõ ràng và cập nhật tiến độ thường xuyên trong dự án nhóm.
- Sử dụng Trello, ClickUp hoặc một công cụ quản lý công việc khác để theo dõi trách nhiệm.
- Tìm hiểu nền tảng RAG trước khi thử nghiệm GraphRAG.
- Tạo knowledge graph nhỏ để hiểu node, edge và graph query.
- Củng cố kỹ năng Linux, networking, troubleshooting và viết tài liệu.
- Xây dựng phòng lab cá nhân và ghi lại các bước cấu hình trong portfolio.
- Tiếp tục học AWS, Docker, automation và Infrastructure as Code.

### Trải nghiệm sự kiện

Tham gia buổi meetup này rất hữu ích vì sự kiện bao gồm nhiều lĩnh vực khác nhau thay vì chỉ tập trung vào một công nghệ.

#### Học hỏi từ nhiều chủ đề kỹ thuật

Phiên Docker cung cấp phần giới thiệu rõ ràng về container và vai trò của chúng trong triển khai ứng dụng. Phiên an ninh mạng kết nối các dịch vụ bảo mật AWS với Machine Learning, phù hợp với chuyên ngành của tôi. Phiên WebSocket cho thấy cách nhiều dịch vụ AWS có thể phối hợp trong một hệ thống thời gian thực.

Phiên GraphRAG giới thiệu một kiến trúc AI mới hơn và giúp tôi hiểu vì sao mối quan hệ giữa các thực thể dữ liệu có thể cải thiện khả năng truy xuất. Phiên System Administrator cung cấp lộ trình nghề nghiệp thực tế, kết nối kỹ năng IT Helpdesk, hạ tầng, cloud và DevOps.

#### Hiểu tầm quan trọng của làm việc nhóm

Phiên làm việc nhóm nhắc tôi rằng kiến thức kỹ thuật chưa đủ để bảo đảm thành công của một dự án. Các thành viên còn cần mục tiêu chung, giao tiếp cởi mở, phân chia nhiệm vụ phù hợp và trách nhiệm cá nhân.

Điều này hữu ích đối với cả dự án học tập và công việc chuyên nghiệp vì nhiều vấn đề kỹ thuật yêu cầu sự phối hợp giữa những người có trách nhiệm khác nhau.

#### Định hướng nghề nghiệp

Sự kiện giúp tôi hiểu rõ hơn một số hướng phát triển nghề nghiệp như:

- Cloud Engineer
- DevOps Engineer
- Cybersecurity Engineer
- System Administrator
- Backend hoặc Serverless Developer
- Artificial Intelligence Engineer

Phiên cuối đặc biệt hữu ích vì cho thấy phát triển nghề nghiệp là một quá trình từng bước. Kỹ năng troubleshooting, Linux, networking, viết tài liệu và kinh nghiệm dự án thực tế có thể tạo nền tảng cho các vị trí Cloud và DevOps nâng cao hơn.

#### Những bài học rút ra

- Việc học nên kết hợp giữa lý thuyết và thực hành.
- Các dự án cá nhân nhỏ có thể giúp biến kiến thức từ workshop thành kỹ năng thực tế.
- Monitoring, security, documentation và teamwork nên được xem xét ngay từ đầu dự án.
- Hiểu rõ một số công nghệ cốt lõi sẽ hiệu quả hơn học nhiều công cụ chỉ ở mức bề mặt.
- Dịch vụ đám mây phát huy hiệu quả nhất khi được lựa chọn dựa trên yêu cầu thực tế của dự án.

### Một số hình ảnh sự kiện

*Thêm hình ảnh sự kiện của bạn tại đây.*
![Hình ảnh sự kiện 1](/images/event-participated/img1.png)

![Hình ảnh sự kiện 2](/images/event-participated/img2.png)

![Hình ảnh sự kiện 3](/images/event-participated/img3.png)

> Nhìn chung, sự kiện giúp tôi có cái nhìn rộng hơn về phát triển phần mềm hiện đại, kiến trúc đám mây, an ninh mạng, trí tuệ nhân tạo, làm việc nhóm và phát triển nghề nghiệp. Sự kiện cũng giúp tôi xác định được những chủ đề thực tế cần tiếp tục học tập và áp dụng vào các dự án AWS và an ninh mạng trong tương lai.