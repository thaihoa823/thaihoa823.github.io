---
title: "Event 3"
date: 2026-07-26
weight: 3
chapter: false
pre: " <b> 4.3. </b> "
---

# Bài thu hoạch sự kiện chia sẻ Agentic AI và hành trình Hackathon AWS

&emsp;**Ngày tham gia:** 26/07/2026  

&emsp;**Vai trò:** Người tham dự  

&emsp;**Nội dung:** Chia sẻ hành trình tham gia Hackathon, xây dựng sản phẩm Agentic AI, thiết kế kiến trúc AWS, tối ưu chi phí và trình diễn các giải pháp thực tế.  

### Mục Đích Của Sự Kiện

* Chia sẻ những kinh nghiệm thực tế trong quá trình tham gia Agentic AI Build Week và các cuộc thi Hackathon liên quan đến AWS.

* Giới thiệu cách các nhóm xác định vấn đề, xây dựng sản phẩm khả dụng tối thiểu và hoàn thành giải pháp trong thời gian giới hạn.

* Trình bày những ứng dụng thực tế của Computer Vision, Generative AI và Agentic AI trong giám sát đám đông, phân tích doanh nghiệp, thiết kế kiến trúc và đặt món trực tuyến.

* Giúp người tham dự hiểu rõ hơn về cách kết hợp các dịch vụ AWS để xây dựng hệ thống có khả năng mở rộng, bảo mật, giám sát và tối ưu chi phí.

* Chia sẻ những khó khăn, bài học, kinh nghiệm làm việc nhóm và phương pháp chuẩn bị cho một cuộc thi Hackathon.

* Tạo động lực cho sinh viên và người mới bắt đầu chủ động tham gia các hoạt động công nghệ, xây dựng sản phẩm và học hỏi từ trải nghiệm thực tế.


### Các Nhóm Và Thành Viên Trình Bày

#### Nhóm 3KA – The Hackathon Journey

* **Huỳnh An Khương**
* **Nguyễn Quốc Huy**
* **Ngô Quang Khôi**
* **Hoàng Lê Thành Đức**
* **Đặng Nguyễn Phước Lộc**
* **Đặng Trường Hưng**

#### Nhóm SignalScout

* **Lê Tấn Lực**
* **Đỗ Hoàng Hiếu**
* **Triệu Quốc Hào**
* **Nguyễn Văn Duy Khiêm**
* **Nguyễn Công Minh**
* **Nguyễn Trần Minh Quân**

#### Nhóm Plan V – Solution Architect Professional AI Native App

* **Phạm Tiến Thuận Phát**
* **Huỳnh Hoàng Long**
* **Lê Minh Nghĩa**
* **Trần Đại Vĩ**
* **Nguyễn An**

#### Nhóm One Team – Colonel AI

* **Anh Duy**
* **Trần Đông**
* **Đoàn Trung**
* **Minh Việt**
* **Anshul Roy**


### Nội Dung Nổi Bật

## 1. The Hackathon Journey – 24 Hours of Building, Failing, and Learning

Bài trình bày của nhóm 3KA chia sẻ toàn bộ hành trình tham gia Hackathon trong vòng 24 giờ. Thay vì chỉ tập trung vào kết quả cuối cùng, nhóm nhấn mạnh những bài học có được trong quá trình xây dựng, gặp lỗi, thay đổi ý tưởng và phối hợp cùng các thành viên.

Hành trình của nhóm được chia thành bốn giai đoạn:

* Đăng ký và lựa chọn chủ đề phù hợp.

* Xây dựng sản phẩm dưới áp lực thời gian.

* Trình bày và demo sản phẩm trước ban giám khảo.

* Tổng kết bài học và rút kinh nghiệm sau cuộc thi.

Nhóm tham gia Hackathon với mục tiêu thử thách bản thân ngoài phạm vi lớp học, có thêm kinh nghiệm thực tế với AI và AWS, học cách xây dựng một sản phẩm hoàn chỉnh trong thời gian ngắn và nâng cao kỹ năng làm việc nhóm.

### Dự án S.H.E.P.H.E.R.D

Nhóm đã phát triển nguyên mẫu mang tên **S.H.E.P.H.E.R.D**, viết tắt của:

**Smart Human-flow Evaluation, Prediction, Hazard Detection, Response, and Dispatch**

Hệ thống được xây dựng nhằm hỗ trợ giám sát mật độ người tại các địa điểm đông người như khu vực ra vào, hàng đợi, gian hàng và khu vực tổ chức sự kiện.

Trong thực tế, nhân viên vận hành phải theo dõi nhiều camera và nhiều khu vực cùng lúc. Phương pháp giám sát thủ công thường có một số hạn chế:

* Phản ứng chậm khi có sự cố.

* Khó mở rộng khi số lượng camera và khu vực tăng lên.

* Có thể bỏ sót những dấu hiệu bất thường.

* Không phản ứng kịp khi điều kiện đám đông thay đổi nhanh chóng.

S.H.E.P.H.E.R.D được xây dựng để phân tích luồng camera trực tiếp và chuyển dữ liệu hình ảnh thành thông tin vận hành rõ ràng.

Các chức năng chính gồm:

* Phát hiện và theo dõi người trong video.

* Đo mật độ đám đông.

* Đánh giá tình trạng hàng đợi.

* Phát hiện các dấu hiệu ùn tắc sớm.

* Dự đoán nguy cơ quá tải.

* Tạo cảnh báo chủ động.

* Đề xuất phương án điều phối nhân viên.

### Công nghệ được sử dụng

* **YOLO** để phát hiện đối tượng trong hình ảnh và video.

* **ByteTrack** để theo dõi đối tượng qua nhiều khung hình.

* **Amazon SageMaker** để hỗ trợ quá trình suy luận trên nền tảng đám mây.

* **Amazon Bedrock AgentCore** và **Strands Agent** để xây dựng lớp Agentic AI.

* **React Monitoring Dashboard** để hiển thị các chỉ số giám sát và cảnh báo.

### Lớp Agentic AI

Giải pháp có hai thành phần Agentic AI quan trọng:

#### Autonomous Monitor

* Liên tục theo dõi các chỉ số đám đông.

* Phát hiện dấu hiệu ùn tắc.

* Dự đoán khả năng quá tải.

* Tự động tạo cảnh báo chủ động.

#### Operator Copilot

* Cho phép nhân viên đặt câu hỏi bằng ngôn ngữ tự nhiên.

* Trả lời dựa trên dữ liệu giám sát trực tiếp.

* Kết hợp các công cụ dự đoán và hành động vận hành.

* Cung cấp câu trả lời ngắn gọn, dễ hiểu và có căn cứ.

### Khó khăn của nhóm

* Chưa có nhiều kiến thức về AI trước khi tham gia.

* Lần đầu làm việc với nhiều dịch vụ AWS.

* Thời gian phát triển rất hạn chế.

* Khó duy trì luồng video trực tiếp ổn định.

* Độ trễ của quá trình suy luận còn cao.

* Khó duy trì việc theo dõi một người qua nhiều khung hình.

* Việc lựa chọn vị trí camera ảnh hưởng đến kết quả phân tích.

* Nhiều lỗi mã nguồn phát sinh trong quá trình xây dựng.

* Phải cân bằng giữa phạm vi chức năng và thời gian hoàn thành.

* Cần làm cho AI Agent có khả năng chủ động, giải thích được và đưa ra hành động phù hợp.

### Bài học từ hành trình Hackathon

Nhóm chia sẻ rằng trước khi tham gia Hackathon cần chuẩn bị:

* Một mục tiêu rõ ràng và xác định sớm tiêu chí hoàn thành.

* Bộ công cụ, tài khoản và mã nguồn mẫu cần thiết.

* Vai trò cụ thể cho từng thành viên như lập trình, thiết kế, thuyết trình và kiểm thử.

* Kịch bản demo ngắn gọn và được luyện tập trước.

* Phạm vi sản phẩm nhỏ nhưng có thể hoàn thành và hoạt động ổn định.

Bài học quan trọng là một sản phẩm nhỏ nhưng hoàn chỉnh sẽ có giá trị hơn một ý tưởng lớn nhưng không thể hoạt động.


## 2. SignalScout – Phân Tích Tín Hiệu Chiến Lược Doanh Nghiệp

SignalScout là nền tảng AI được xây dựng nhằm phát hiện sớm những thay đổi chiến lược và dấu hiệu tái cấu trúc trong doanh nghiệp.

Trong thực tế, các thông tin về một doanh nghiệp thường nằm rải rác ở nhiều nguồn khác nhau. Việc thu thập, kiểm tra và liên kết những thông tin này thành một kết luận đáng tin cậy thường mất nhiều thời gian.

SignalScout hướng đến việc:

* Thu thập và xác minh các bằng chứng liên quan đến doanh nghiệp.

* Phát hiện sớm những thay đổi chiến lược.

* Nhận diện tín hiệu tái cấu trúc tổ chức.

* Phân tích các chỉ số tài chính và vận hành.

* Xây dựng các kịch bản có thể xảy ra.

* Kết nối những tín hiệu rời rạc thành một câu chuyện rõ ràng.

* Cung cấp bằng chứng cho từng kết luận.

* Hỗ trợ doanh nghiệp đưa ra quyết định Maintain, Adapt hoặc Accelerate.

### Nhóm người dùng mục tiêu

* Bộ phận chiến lược doanh nghiệp.

* Bộ phận quản lý rủi ro.

* Bộ phận phân tích đối thủ cạnh tranh.

* Nhóm quản lý khách hàng doanh nghiệp B2B.

### Giá trị của giải pháp

* Cung cấp dashboard tự phục vụ cho người dùng.

* Trình bày báo cáo phân tích, dòng thời gian và cảnh báo rủi ro.

* Tạo ra kết quả minh bạch và có thể kiểm chứng.

* Hỗ trợ quyết định nhưng vẫn giữ con người ở vị trí kiểm soát cuối cùng.

* Không chỉ đưa ra kết luận mà còn cung cấp các bằng chứng hỗ trợ.

### Công nghệ và đối tác

Giải pháp kết hợp hệ sinh thái AWS với một số nền tảng hỗ trợ:

* Amazon Bedrock.

* Amazon Bedrock AgentCore.

* AWS WAF.

* AWS Amplify Hosting.

* Amazon CloudWatch.

* AWS Secrets Manager.

* Amazon DynamoDB.

* AWS Lambda.

* Amazon Route 53.

* AWS CloudTrail.

* Amazon S3 Intelligent-Tiering.

* Amazon API Gateway.

* Amazon Cognito.

* Langfuse.

* TinyFish.

* Apify.

### Phân tích và tối ưu chi phí

Nhóm không chỉ xây dựng chức năng mà còn thực hiện ước tính chi phí cho nhiều mức sử dụng khác nhau.

Theo phần trình bày, tổng chi phí dịch vụ AWS được ước tính trong khoảng:

* Mức thấp: khoảng **17 USD mỗi tháng**.

* Mức trung bình: khoảng **35 USD mỗi tháng**.

* Mức cao: khoảng **130 USD mỗi tháng**.

Khi tính thêm các nền tảng bên ngoài như Apify, TinyFish và Langfuse, tổng chi phí dự kiến dao động từ khoảng **81 USD đến 359 USD mỗi tháng**.

Nhóm cũng đề xuất một kiến trúc tiết kiệm chi phí hơn, cho thấy việc thiết kế hệ thống cần cân bằng giữa khả năng xử lý, độ tin cậy và ngân sách vận hành.


## 3. Solution Architect Professional AI Native App

Bài trình bày của nhóm Plan V tập trung vào việc ứng dụng Agentic AI để hỗ trợ công việc của một Solution Architect.

Trong quá trình tư vấn giải pháp, Solution Architect thường phải thực hiện nhiều công việc thủ công:

* Đọc tài liệu BRD hoặc PRD từng dòng.

* Trích xuất và phân loại yêu cầu.

* Xác định những yêu cầu còn thiếu.

* Xây dựng kiến trúc ban đầu từ một trang trống.

* Vẽ sơ đồ kiến trúc.

* Ước tính chi phí đám mây ở mức tổng quan.

* Viết Infrastructure as Code.

* Điều chỉnh kiến trúc theo phản hồi của khách hàng.

Các công việc này cần nhiều kinh nghiệm và có thể mất nhiều thời gian, đặc biệt khi khách hàng yêu cầu kết quả trong thời gian ngắn.

### Giải pháp được đề xuất

Nhóm phát triển **Solution Architect Professional AI Native App**, một ứng dụng AI có khả năng:

* Phân tích yêu cầu được mô tả bằng ngôn ngữ tự nhiên.

* Phân tích tài liệu yêu cầu có cấu trúc.

* Xây dựng danh mục yêu cầu trong thời gian ngắn.

* Đề xuất nhiều phương án kiến trúc ở mức tổng quan.

* Hỗ trợ cả kiến trúc AWS và kiến trúc Hybrid Cloud.

* Điều chỉnh đề xuất theo tiêu chuẩn của doanh nghiệp.

* Tạo sơ đồ Draw.io có thể tiếp tục chỉnh sửa.

* Sử dụng các biểu tượng kiến trúc AWS chính thức.

* Đưa ra ước tính chi phí định hướng cho Region `ap-southeast-1`.

* Hiển thị các đề xuất, giả định và khoảng trống trong yêu cầu.

* Cho phép người dùng trao đổi và tinh chỉnh kiến trúc qua giao diện chat.

* Hỗ trợ custom instruction riêng cho từng dự án.

* Hỗ trợ tự động tạo Infrastructure as Code.

### Tác động của giải pháp

Trước khi sử dụng ứng dụng:

* Solution Architect phải đọc BRD hoặc PRD thủ công.

* Mỗi kiến trúc thường được bắt đầu từ một trang trống.

* Infrastructure as Code phải được viết thủ công.

* Chi phí thường được ước tính dựa nhiều vào kinh nghiệm cá nhân.

Sau khi sử dụng ứng dụng:

* Người dùng có thể tải tài liệu lên và trao đổi bằng ngôn ngữ tự nhiên.

* Hệ thống tạo Requirements Catalogue trong thời gian ngắn.

* Solution Architect nhận được một bản kiến trúc đầu tiên có căn cứ để đánh giá và chỉnh sửa.

* Infrastructure as Code có thể được tạo tự động.

* Ước tính chi phí được tạo cùng với phương án kiến trúc.

Điểm quan trọng là AI không thay thế hoàn toàn Solution Architect. AI hỗ trợ xử lý những công việc lặp lại và tạo bản nháp đầu tiên, trong khi chuyên gia vẫn chịu trách nhiệm kiểm tra, điều chỉnh và đưa ra quyết định cuối cùng.


## 4. Colonel AI – AI-Powered Conversational Ordering

Bài trình bày của One Team giới thiệu hành trình xây dựng **KFC Bot Agent**, một AI Agent hỗ trợ đặt món trên nhiều kênh giao tiếp.

Thay vì yêu cầu người dùng rời khỏi cuộc trò chuyện, tải ứng dụng, tạo tài khoản và thực hiện nhiều bước đặt hàng, giải pháp cho phép khách hàng đặt món ngay trong kênh nhắn tin đang sử dụng.

Các kênh được định hướng hỗ trợ gồm:

* Zalo Official Account.

* Messenger.

* WhatsApp.

* Các kênh giao tiếp có thể được bổ sung trong tương lai.

### Thách thức của đặt món bằng hội thoại

Đặt món không chỉ là một bài toán hỏi đáp thông thường. AI cần hiểu chính xác:

* Tên món ăn.

* Số lượng.

* Kích thước và các biến thể của sản phẩm.

* Quy tắc áp dụng voucher.

* Trạng thái hiện tại của giỏ hàng.

* Các trường hợp lỗi.

* Quy định kinh doanh của doanh nghiệp.

* Yêu cầu xác nhận đơn hàng.

Một chatbot thông thường có thể tạo câu trả lời, nhưng một AI Agent cần thực hiện hành động dựa trên dữ liệu kinh doanh thật.

Quy trình hoạt động được trình bày gồm:

1. Xác định mục tiêu của người dùng.

2. Lập kế hoạch các bước cần thực hiện.

3. Lựa chọn công cụ phù hợp.

4. Thực hiện hành động.

5. Kiểm tra kết quả trước khi xác nhận.

Agent cần hiểu ý định đặt món, tìm kiếm dữ liệu kinh doanh đáng tin cậy, cập nhật giỏ hàng, áp dụng chương trình khuyến mãi và xác minh đơn hàng thực tế.

### Chuyển đổi từ Monolithic sang Microservices

Bài trình bày cũng so sánh hai mô hình kiến trúc:

#### Monolithic Architecture

* Toàn bộ chức năng nằm trong một codebase lớn.

* Các thành phần liên kết chặt chẽ.

* Chu kỳ phát hành chậm.

* Khó mở rộng riêng từng chức năng.

* Các nhóm phát triển phụ thuộc nhiều vào nhau.

#### Microservices Architecture

* Hệ thống được chia thành các dịch vụ nhỏ và độc lập.

* Mỗi dịch vụ quản lý logic và dữ liệu riêng.

* Các dịch vụ có thể được triển khai độc lập.

* Hỗ trợ phát triển và cải tiến nhanh hơn.

* Có khả năng mở rộng tốt hơn.

### Kiến trúc đa kênh

Giải pháp được thiết kế theo nguyên tắc:

**Design Once – Deploy Everywhere**

Khi cần hỗ trợ thêm một kênh giao tiếp mới, nhóm chỉ cần bổ sung adapter. Khi cần kết nối với một hệ thống kinh doanh mới, nhóm có thể thêm connector. Khi cần một chức năng mới, nhóm có thể bổ sung tool cho Agent.

Cách thiết kế này giúp hệ thống thay đổi và mở rộng mà không phải xây dựng lại toàn bộ ứng dụng.

### Kết quả được trình bày

Theo số liệu ước tính của nhóm:

* Chi phí trung bình khoảng **0,006 USD cho mỗi đơn hàng**.

* Tổng chi phí hạ tầng khoảng **88 USD mỗi tháng** với 500 đơn hàng mỗi ngày.

* Độ trễ từ khi người dùng gửi tin nhắn đến khi nhận được phản hồi khoảng **3–5 giây**.

* Amazon Bedrock chiếm phần lớn chi phí vận hành.

* Việc sử dụng AgentCore giúp giảm khoảng **60% mã nguồn hạ tầng**.

Giải pháp cho thấy Agentic AI có thể được ứng dụng vào quy trình kinh doanh thực tế, nhưng cần kết hợp với dữ liệu đáng tin cậy, quy tắc nghiệp vụ rõ ràng và bước xác minh trước khi thực hiện giao dịch.


### Những Gì Học Được

#### Tư duy xây dựng sản phẩm

* Cần bắt đầu từ một vấn đề thực tế thay vì lựa chọn công nghệ trước.

* Phạm vi sản phẩm phải phù hợp với thời gian và nguồn lực của nhóm.

* Một sản phẩm nhỏ nhưng hoạt động ổn định có giá trị hơn một sản phẩm có quá nhiều chức năng nhưng không thể hoàn thành.

* Cần xác định rõ tiêu chí hoàn thành ngay từ đầu.

* Demo phải được xem là một phần của sản phẩm chứ không phải công việc thực hiện ở phút cuối.

#### Kiến thức về Agentic AI

* AI Agent khác chatbot ở khả năng lập kế hoạch, sử dụng công cụ, thực hiện hành động và xác minh kết quả.

* Agent chỉ nên thực hiện hành động dựa trên dữ liệu đáng tin cậy.

* Hệ thống cần có cơ chế kiểm soát của con người đối với các quyết định quan trọng.

* Một AI Agent tốt cần chủ động, giải thích được và đưa ra hành động phù hợp.

* Agentic AI có thể được ứng dụng trong giám sát, phân tích doanh nghiệp, thiết kế kiến trúc và thương mại điện tử.

#### Kiến thức về kiến trúc AWS

* Microservices giúp tách biệt chức năng và hỗ trợ triển khai độc lập.

* Kiến trúc cần được thiết kế để có thể bổ sung kênh, hệ thống hoặc công cụ mới.

* Amazon Bedrock và AgentCore có thể hỗ trợ xây dựng ứng dụng Agentic AI.

* CloudWatch và CloudTrail hỗ trợ giám sát, truy vết và kiểm tra hoạt động.

* AWS WAF, Cognito và Secrets Manager có vai trò quan trọng trong bảo mật ứng dụng.

* Lambda, DynamoDB, API Gateway và S3 phù hợp với các workload có kiến trúc serverless.

* Việc lựa chọn Region ảnh hưởng đến độ trễ, khả năng tích hợp và chi phí.

#### Kiến thức về chi phí

* Ước tính chi phí cần được thực hiện ngay trong giai đoạn thiết kế.

* Chi phí mô hình AI và token có thể chiếm phần lớn ngân sách vận hành.

* Không nên chỉ tính chi phí AWS mà cần tính cả các dịch vụ bên ngoài.

* Cần xây dựng nhiều kịch bản chi phí tương ứng với lượng người dùng thấp, trung bình và cao.

* Tối ưu kiến trúc không chỉ nhằm giảm giá mà còn phải duy trì hiệu năng và độ tin cậy.

#### Kỹ năng làm việc nhóm

* Các thành viên cần được phân công vai trò rõ ràng.

* Nhóm cần thống nhất cách quản lý mã nguồn và quy trình commit.

* Không được đưa tệp chứa thông tin nhạy cảm như `.env` lên kho mã nguồn công khai.

* Cần giao tiếp thường xuyên để tránh trùng lặp hoặc bỏ sót công việc.

* Một nhóm có nhiều kỹ năng khác nhau thường hiệu quả hơn một nhóm có các thành viên cùng làm một nhiệm vụ.

* Cần dành thời gian luyện tập phần thuyết trình và demo.


### Ứng Dụng Vào Học Tập Và Công Việc

* Áp dụng phương pháp xác định vấn đề và giới hạn phạm vi trước khi bắt đầu một dự án AWS.

* Xây dựng sản phẩm theo hướng MVP, ưu tiên hoàn thành một luồng chính trước khi bổ sung chức năng nâng cao.

* Phân chia hệ thống thành các thành phần độc lập để dễ phát triển, kiểm thử và mở rộng.

* Sử dụng AWS Architecture Icons và Draw.io để trình bày kiến trúc rõ ràng.

* Tạo bảng giả định và ước tính chi phí ngay khi thiết kế kiến trúc.

* Sử dụng Amazon CloudWatch để theo dõi log, metric và lỗi của hệ thống.

* Áp dụng AWS WAF, Amazon Cognito và Secrets Manager để tăng cường bảo mật.

* Nghiên cứu Amazon Bedrock và AgentCore để xây dựng các tính năng Agentic AI.

* Thiết kế AI Agent theo quy trình hiểu mục tiêu, lập kế hoạch, sử dụng công cụ, thực hiện và xác minh.

* Giữ con người ở vị trí kiểm soát cuối cùng đối với các hành động quan trọng.

* Chuẩn bị tài khoản, công cụ, mã nguồn mẫu và kịch bản demo trước khi tham gia Hackathon.

* Quản lý mã nguồn cẩn thận, không commit access key, secret key hoặc tệp `.env`.

* Phân công thành viên phụ trách lập trình, kiến trúc, giao diện, kiểm thử và thuyết trình.


### Trải Nghiệm Trong Sự Kiện

Tham gia sự kiện ngày 26/07/2026 là một trải nghiệm bổ ích, giúp tôi tiếp cận nhiều góc nhìn khác nhau về việc xây dựng sản phẩm với AI và AWS.

#### Học hỏi từ các dự án thực tế

Bốn bài trình bày không chỉ giới thiệu ý tưởng mà còn phân tích vấn đề, giải pháp, kiến trúc, chi phí, khó khăn và kết quả demo. Qua đó, tôi hiểu rõ hơn quá trình chuyển một ý tưởng ban đầu thành một sản phẩm có thể hoạt động.

Dự án S.H.E.P.H.E.R.D cho thấy cách kết hợp Computer Vision, theo dõi đối tượng và Agentic AI để giải quyết bài toán giám sát đám đông.

SignalScout cho thấy AI có thể hỗ trợ doanh nghiệp thu thập bằng chứng, kết nối dữ liệu và phát hiện những thay đổi chiến lược.

Solution Architect Professional AI Native App minh họa cách AI hỗ trợ phân tích yêu cầu, tạo kiến trúc, vẽ sơ đồ, xây dựng Infrastructure as Code và ước tính chi phí.

Colonel AI cho thấy AI Agent có thể thực hiện một quy trình kinh doanh thực tế trên nhiều kênh giao tiếp.

#### Hiểu rõ khó khăn khi xây dựng sản phẩm

Các nhóm đã chia sẻ thẳng thắn về nhiều khó khăn như thiếu kinh nghiệm AI, lần đầu sử dụng AWS, thời gian hạn chế, lỗi mã nguồn, độ trễ, chi phí và áp lực hoàn thành demo.

Những chia sẻ này giúp tôi nhận ra rằng việc gặp lỗi và thay đổi kế hoạch là một phần bình thường của quá trình phát triển sản phẩm. Điều quan trọng là phải xác định đúng ưu tiên và hoàn thành một luồng hoạt động chính.

#### Thay đổi tư duy về Hackathon

Trước đây, tôi thường xem Hackathon chủ yếu là một cuộc thi lập trình. Sau sự kiện, tôi hiểu rằng Hackathon còn là cơ hội để:

* Kiểm tra khả năng giải quyết vấn đề.

* Làm việc trong điều kiện thời gian giới hạn.

* Học công nghệ mới nhanh chóng.

* Giao tiếp và phân chia công việc trong nhóm.

* Trình bày ý tưởng trước người khác.

* Kết nối với những người có cùng sở thích công nghệ.

* Nhận ra khả năng thực tế của bản thân.

#### Bài học cá nhân

Bài học lớn nhất tôi rút ra là không cần chờ đến khi có đầy đủ kiến thức mới bắt đầu. Việc chủ động tham gia, thử nghiệm và hoàn thành một sản phẩm nhỏ sẽ mang lại nhiều kinh nghiệm hơn so với chỉ học lý thuyết.

Tôi cũng nhận thấy kiến trúc, chi phí, bảo mật và khả năng demo cần được xem xét ngay từ đầu. Một giải pháp kỹ thuật tốt không chỉ cần hoạt động mà còn phải dễ giải thích, có khả năng mở rộng và phù hợp với nhu cầu thực tế.


### Một Số Hình Ảnh Khi Tham Gia Sự Kiện

![Bài trình bày The Hackathon Journey của nhóm 3KA](/images/event-participated/event3.1.png)

![Bài trình bày SignalScout](/images/event-participated/event3.2.png)

![Bài trình bày Solution Architect Professional AI Native App](/images/event-participated/event3.3.png)


> Tổng thể, sự kiện giúp tôi hiểu rõ hơn về quá trình xây dựng sản phẩm Agentic AI trên AWS, từ xác định vấn đề, thiết kế kiến trúc, phát triển MVP và kiểm thử đến ước tính chi phí, trình bày sản phẩm và rút kinh nghiệm sau Hackathon.