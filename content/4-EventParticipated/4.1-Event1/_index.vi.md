---
title: "Event 1"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 4.1. </b> "
---



# Bài thu hoạch “Automated Prompt Engineering:Enhancing LLM Output Quality”

### Mục Đích Của Sự Kiện

- Giới thiệu khái niệm và vai trò của Prompt Engineering trong việc nâng cao chất lượng đầu ra của các Mô hình Ngôn ngữ Lớn (LLMs).
- Chia sẻ các phương pháp và kỹ thuật xây dựng prompt hiệu quả nhằm cải thiện độ chính xác, tính nhất quán và khả năng suy luận của AI.
- Trình bày các kỹ thuật tự động hóa Prompt Engineering để tối ưu hóa hiệu suất và giảm sự can thiệp thủ công.
- Giới thiệu các công cụ và giải pháp AI hỗ trợ phát triển, kiểm thử và tối ưu prompt trong quá trình xây dựng ứng dụng AI.
- Trao đổi các kinh nghiệm thực tế và xu hướng ứng dụng LLM trong phát triển phần mềm và các bài toán doanh nghiệp.
### Danh Sách Diễn Giả

### Diễn giả

- **Long Hoang** - Diễn giả,  Amazon Web Services (AWS).
- **Thinh Nguyen** - Diễn giả, Amazon Web Services (AWS).
- **Khang Nguyen** - Diễn giả, Associate Specialist Solutions Architect (Serverless), Amazon Web Services (AWS).
- **Thao Nguyen Phuong** - Diễn giả, Associate Specialist Solutions Architect (Serverless), Amazon Web Services (AWS).

### Nội Dung Nổi Bật

#### Những hạn chế khi Prompt Engineering chưa hiệu quả

- Prompt quá chung chung → AI tạo ra kết quả chung chung, thiếu chiều sâu.
- Thiếu ngữ cảnh → Câu trả lời không đúng với yêu cầu hoặc mục tiêu.
- Hướng dẫn mơ hồ → Kết quả không nhất quán giữa các lần thực hiện.
- Tiêu tốn nhiều token → Gia tăng chi phí sử dụng mô hình AI.
- Không quy định định dạng đầu ra → Khó xử lý và tích hợp vào ứng dụng.
- Thiếu ví dụ minh họa (Few-shot) → Giảm độ chính xác của kết quả.
- Thiếu ràng buộc (Constraints) → AI có thể tạo nội dung dài dòng hoặc không đúng trọng tâm.

#### Học tập và thực hành AWS dành cho người mới bắt đầu


- Giới thiệu **Free Hands-on Learning Playground** – môi trường thực hành miễn phí giúp người học trải nghiệm các dịch vụ AWS mà không cần triển khai trên tài khoản thật.
- Phân tích những khó khăn thường gặp của người mới bắt đầu với AWS, như cấu hình dịch vụ, quản lý tài nguyên, chi phí và quyền truy cập (IAM).
- Trình bày phương pháp **Local AWS Testing**, cho phép phát triển và kiểm thử ứng dụng AWS ngay trên máy tính cá nhân trước khi triển khai lên môi trường Cloud.
- So sánh hai công cụ **LocalStack** và **Floci**, bao gồm khả năng mô phỏng các dịch vụ AWS, tốc độ, tính tương thích và các trường hợp sử dụng phù hợp trong quá trình phát triển và kiểm thử ứng dụng.
#### Hack Não Để Học Như Nghiện Game

- Phân tích nguyên nhân tâm lý: Não bộ ưu tiên hoạt động tiêu hao ít năng lượng, phần thưởng đến nhanh và kích thích tính tò mò — đây đều là đặc tính cốt lõi mà mạng xã hội và game online đã khai thác triệt để.
- Cơ chế dopamine: Dopamine không được tiết ra khi nhận phần thưởng, mà tiết ra khi kỳ vọng phần thưởng sắp đến. Đây chính là lý do các thuật toán TikTok và cơ chế slot machine giữ chân người dùng hiệu quả đến vậy.
- Kỹ thuật "hộp phần thưởng bí ẩn": Viết nhiều phần thưởng nhỏ ngẫu nhiên vào từng tờ giấy, bỏ vào hộp, cứ mỗi 10 phút học thì bốc một tờ. Sự tò mò về phần thưởng tiếp theo sẽ kích thích não bộ tiết dopamine liên tục, giúp duy trì động lực.
- Khai thác nỗi sợ mất mát: Dùng lịch điểm danh học tập hàng ngày như hệ thống "chuỗi streak" của Duolingo hay điểm danh sự kiện trong game. Khi chuỗi đã dài, bạn sẽ sợ gãy chuỗi hơn là lười học.
- Chia nhỏ nhiệm vụ: Chia nội dung học thành các phần nhỏ, mỗi ngày một dịch vụ AWS thay vì cố học tất cả trong một buổi. Tương tự như cách một người mới tập chạy chia lộ trình 5km thành nhiều chặng ngắn.
### Ứng dụng AI Prompt trong phát triển ứng dụng trên AWS

- Giới thiệu cách sử dụng AI Prompt để hỗ trợ xây dựng và phát triển các ứng dụng trên nền tảng AWS.
- Hướng dẫn sử dụng AI để sinh mã nguồn (code generation), giải thích mã, sửa lỗi và tối ưu chương trình.
- Ứng dụng AI Prompt trong việc thiết kế kiến trúc hệ thống, tạo tài liệu kỹ thuật và hỗ trợ triển khai các dịch vụ AWS.
- Trình bày cách sử dụng AI để tạo các ứng dụng mẫu, API, chatbot và các giải pháp Serverless trên AWS.
- Chia sẻ các nguyên tắc viết Prompt hiệu quả nhằm nâng cao chất lượng kết quả và tăng năng suất phát triển phần mềm.
- Minh họa các tình huống thực tế khi kết hợp AI với các công cụ của AWS để rút ngắn thời gian phát triển và kiểm thử ứng dụng.

### Những Gì Học Được

#### Tư Duy Thiết Kế

- Hiểu được tầm quan trọng của Prompt Engineering trong việc nâng cao chất lượng đầu ra của các mô hình ngôn ngữ lớn (LLMs).
- Biết cách xây dựng prompt theo cấu trúc gồm Role, Instruction, Context, Input, Output Format, Examples và Constraints.
- Nhận thức được việc thiết kế prompt tốt giúp giảm chi phí, tiết kiệm thời gian và nâng cao hiệu quả làm việc với AI.


#### Kiến Thức Kỹ Thuật

- Hiểu nguyên lý hoạt động của Prompt Engineering và Automated Prompt Engineering.
- Biết cách tối ưu prompt để tăng độ chính xác và tính nhất quán của kết quả.
- Tìm hiểu về Local AWS Testing giúp phát triển và kiểm thử ứng dụng ngay trên máy tính cá nhân.
- Hiểu sự khác biệt giữa LocalStack và Floci trong việc mô phỏng các dịch vụ AWS.
- Biết cách ứng dụng AI Prompt vào việc sinh mã nguồn, giải thích mã, tạo tài liệu và hỗ trợ phát triển ứng dụng trên AWS.

#### Xu Hướng Ứng Dụng AI

- AI hỗ trợ lập trình và phát triển phần mềm ngày càng phổ biến.
- Prompt Engineering trở thành kỹ năng quan trọng đối với lập trình viên khi làm việc với các mô hình AI.
- Các công cụ AI giúp rút ngắn thời gian phát triển, kiểm thử và triển khai ứng dụng.
- AWS đang tích hợp nhiều giải pháp AI nhằm hỗ trợ lập trình viên nâng cao năng suất làm việc.

---

### Ứng Dụng Vào Công Việc

- Áp dụng kỹ thuật Prompt Engineering để sử dụng AI hiệu quả trong học tập và phát triển phần mềm.
- Sử dụng AI để hỗ trợ sinh mã nguồn, giải thích lỗi và tối ưu chương trình.
- Ứng dụng LocalStack hoặc Floci để kiểm thử các dịch vụ AWS trước khi triển khai lên môi trường Cloud.
- Vận dụng AI trong việc thiết kế kiến trúc, tạo tài liệu kỹ thuật và xây dựng các ứng dụng trên nền tảng AWS.

---

### Trải Nghiệm Trong Event

#### Học hỏi từ các diễn giả có chuyên môn cao

- Được lắng nghe những chia sẻ thực tế từ các chuyên gia của Amazon Web Services (AWS).
- Tiếp cận nhiều kinh nghiệm về Prompt Engineering, AI và phát triển ứng dụng trên nền tảng AWS.

#### Trải nghiệm kỹ thuật thực tế

- Được giới thiệu các tình huống thực tế khi sử dụng AI trong phát triển phần mềm.
- Hiểu rõ hơn quy trình xây dựng Prompt và cách tối ưu chất lượng đầu ra của mô hình AI.

#### Ứng dụng công cụ hiện đại

- Làm quen với các công cụ AI hỗ trợ lập trình và phát triển ứng dụng.
- Tìm hiểu các giải pháp kiểm thử cục bộ như LocalStack và Floci trước khi triển khai lên AWS.

#### Kết nối và trao đổi

- Có cơ hội trao đổi với các diễn giả và những người tham dự về AI và AWS.
- Học hỏi thêm nhiều kinh nghiệm và phương pháp làm việc từ cộng đồng công nghệ.

#### Bài học rút ra

- Prompt Engineering là một kỹ năng quan trọng khi làm việc với các mô hình AI hiện đại.
- Việc cung cấp đầy đủ ngữ cảnh và yêu cầu rõ ràng giúp AI tạo ra kết quả chính xác và chất lượng hơn.
- Kết hợp AI với các dịch vụ AWS giúp nâng cao hiệu quả phát triển phần mềm, giảm thời gian triển khai và tối ưu chi phí.

---

#### Một số hình ảnh khi tham gia sự kiện

{{< figure src="/images/4-Event/event1.jpg" title="" >}}

> **Tổng kết:** Buổi chia sẻ giúp tôi hiểu rõ hơn về Prompt Engineering và vai trò của AI trong phát triển phần mềm hiện đại. Đồng thời, tôi cũng tiếp cận được các công cụ và phương pháp mới giúp nâng cao hiệu quả làm việc với AWS, từ đó có thêm nhiều kiến thức và kinh nghiệm để áp dụng vào học tập cũng như các dự án thực tế trong tương lai.