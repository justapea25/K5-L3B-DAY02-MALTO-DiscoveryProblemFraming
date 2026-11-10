# Team

> Điền file này trên repo chung do nhóm trưởng fork. Nhóm điền phần **Thông tin nhóm** và **Thành viên**. Mỗi người tự kiểm tra phần **Cá nhân** của mình. Không copy file này sang repo khác.

## Thông tin nhóm

- **Tên nhóm:** MALTO
- **Candidate problem nhóm chọn (1 câu):** Hệ thống Computer Vision hỗ trợ phát hiện sớm và cảnh báo dấu hiệu sự cố thú cưng tại khu chung cư/khu đô thị để BQL và an ninh xác minh, xử lý.
- **Phạm vi cuối cùng:** Phóng uế, chó không đeo rọ mõm tại khu vực có yêu cầu và hành vi có dấu hiệu gây thương tích; AI **không** tự xác định căn hộ hoặc chủ sở hữu, **không** tự xử phạt.
- **Quyết định cuối (Go / Not Yet / No-Go):** **Not Yet** đối với triển khai thương mại; **Go có điều kiện** đối với pilot nhỏ.

## Thành viên

| STT | Họ và tên | MSSV | Vai trò trong nhóm | Tài khoản GitHub |
|---:|---|---|---|---|
| 1 | Đậu Hoàng Minh | 2A202604011 | Nhóm trưởng; thiết kế slide; phụ trách CP6 — mức can thiệp AI | `justapea25` |
| 2 | Nguyễn Xuân Khánh Linh | 2A202603801 | Điều phối thảo luận CP3–CP4; lập bảng tiêu chí chọn candidate; Assumption Map và hỗ trợ research | `linkiewinkie` |
| 3 | Đặng Minh Thu | 2A202604009 | Research công nghệ; phân tích quy trình trước/sau (CP5) | `minhthu27` |
| 4 | Lê Thế Anh | 2A202603983 | Đề xuất bài toán thú cưng; Problem Statement v1, tiêu chí đánh giá và quyết định CP6 | `LETHESHIYING` |

*Không công khai email/số điện thoại trong bảng này.*

## Phân công theo checkpoint

| Checkpoint | Người chính | Người hỗ trợ | Sản phẩm |
|---|---|---|---|
| CP3 — Hội tụ nhóm | Nguyễn Xuân Khánh Linh | Đậu Hoàng Minh; các thành viên góp candidate | Cluster, cây OST, bảng chấm theo 7 tiêu chí, lý do chọn |
| CP4 — Kiểm chứng | Nguyễn Xuân Khánh Linh | Lê Thế Anh (cung cấp phản ánh cư dân) | Assumption Map, câu hỏi phỏng vấn, snapshot / survey khi có dữ liệu |
| CP4 — Research | Đặng Minh Thu | Nguyễn Xuân Khánh Linh; Đậu Hoàng Minh rà nội dung thuyết trình | Bảng research Frigate, AXIS, NVIDIA có nguồn và khoảng trống |
| CP5 — Quy trình trước/sau | Đặng Minh Thu | Đậu Hoàng Minh (slide quy trình) | Workflow As-Is/To-Be và so sánh before/after |
| CP5 — Problem Statement v0 | Đặng Minh Thu | Đặng Minh Thu; Lê Thế Anh | Problem Statement v0 |
| CP6 — Mức can thiệp + Problem Statement v1 | Đậu Hoàng Minh | Lê Thế Anh | Ma trận, AI Canvas, PAIR, evaluation, Problem Statement v1 |
| CP6 — Quyết định | Lê Thế Anh | Đậu Hoàng Minh | Bốn rủi ro + Go / Not Yet / No-Go |

## Cá nhân

### Đậu Hoàng Minh - 2A202604011

**Phần việc phụ trách:**

- Mục 6 — Mức can thiệp AI (ma trận độ mơ hồ × độ phức tạp, so sánh 4 mức, AI Canvas, 2 câu hỏi Google PAIR).
- Mục 9 — Hạn chế và hướng tiếp theo.
- Slide pitch (7 trang), gồm quy trình hiện tại và quy trình 3 bước trong bản phác thảo.
- Phân tích các ý kiến problem, đưa ra giải pháp kỹ thuật cho problem đề ra.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Ở giai đoạn chọn đề tài: pitch card tổng hợp sau cuộc họp, phản biện card của các bạn khác.
- Đề xuất tách bài toán truy vết sự cố thú cưng thành 3 bước: (1) phát hiện sự kiện, (2) xác nhận thú cưng, (3) truy vết căn hộ, thay vì cho AI nhận diện thẳng căn hộ từ video. Nhờ đó nhóm thấy bottleneck có thể nằm ở bước tìm đoạn video và cần thu hẹp phạm vi AI.
- Viết bản đầu mục 6: ma trận độ mơ hồ × độ phức tạp, lập luận vì sao No AI và Rule chưa đủ, vì sao không cần Agent, và chọn Workflow; AI Canvas và phân tích báo nhầm/bỏ sót. Bản cuối được nhóm điều chỉnh theo phạm vi phát hiện và cảnh báo sớm.
- Viết mục 9: liệt kê hạn chế về bằng chứng, dữ liệu camera, quyền riêng tư, phạm vi giải pháp, đề xuất hướng tiếp theo.
- Làm slide pitch 7 trang cho bài thuyết trình.

**Bằng chứng:**

- Mục 6 và Mục 9 trong file `report/team/group_report.md`.
- File `report/assets/cp5-workflow-current.png` (quy trình hiện tại trong slide pitch).
- Commit `77c2f95` (thêm mục 6, mục 9), `aa3677e` (gộp báo cáo của các thành viên).
- [Báo cáo cá nhân](report/individual/2A202604011_DauHoangMinh.md).

**Điều mình học được từ phần nhóm:**

Mình học được rằng chọn mức AI phải đi từ mức đơn giản nhất và chỉ áp dụng khi cần thiết. Lúc đầu cả nhóm có suy nghĩ AI làm hết cho cả quy trình nhận diện thú cưng vi phạm, nhưng khi vẽ lại quy trình thì thấy chỉ cần AI ở đúng bước phù hợp, còn quyết định xử lý phải để con người làm. Mình cũng học được là cùng một lỗi của AI có thể rẻ ở bước này nhưng rất đắt ở bước khác: bỏ sót đoạn video thì tốn công, nhưng nêu nhầm căn hộ có thể gây mâu thuẫn. Cuối cùng, việc card của mình bị loại vì đã có nhiều tool giải quyết giúp mình hiểu một problem tốt không chỉ cần pain thật mà còn phải có khoảng trống thật.

### Nguyễn Xuân Khánh Linh - 2A202603801

**Phần việc phụ trách:**

- Điều phối công việc và thảo luận CP3–CP4.
- Lập bảng tiêu chí đánh giá candidate theo bảy yếu tố của rubric CP3 và hỗ trợ nhóm chọn vấn đề.
- Chuẩn bị Assumption Map, bộ câu hỏi kiểm chứng theo The Mom Test; tổng hợp research và lý do thu hẹp problem ở CP4.

**Đóng góp cụ thể:**

- Chuẩn bị ba Problem Cards cá nhân: creative chờ test, thiết lập remote key lặp lại và hỗ trợ sửa IELTS Writing. Đưa các candidate này vào quá trình cân nhắc
- Khi phản biện ý tưởng của thành viên khác, đặt câu hỏi: “Ứng dụng này chỉ sửa UI/UX à bạn?” và “Ứng dụng này khác gì dùng ChatGPT để sửa CV?” Các câu hỏi nhằm phân biệt vấn đề thực sự và điểm khác biệt so với giải pháp có sẵn.
- Lập bảng chấm 7 tiêu chí: actor rõ, workflow rõ, pain có bằng chứng, impact đo được, vừa sức lab, so sánh được 4 mức AI, nhóm hiểu domain.
- Điều phối trình tự thảo luận từ shortlist, xác định giả định, research đến điều chỉnh phạm vi.
- Soạn Assumption Map, câu hỏi phỏng vấn và phần research công nghệ Frigate NVR, AXIS Object Analytics, NVIDIA DeepStream; lưu ý phát hiện chó/mèo chưa đồng nghĩa với phát hiện vi phạm.
- Góp ý điều chỉnh ý tưởng từ phát hiện/truy vết/xác định căn hộ thành **cảnh báo dấu hiệu nghi vấn**, để nhân viên an ninh xác minh và BQL xử lý. Bỏ mục thất lạc; tập trung phóng uế, không rọ mõm và dấu hiệu gây thương tích.

**Bằng chứng:**

- [Báo cáo cá nhân của Linh](report/individual/2A202603801_NguyenXuanKhanhLinh.md), nhất là mục CP3–CP4.
- Mục 2 (CP3) và mục 3 (CP4) trong [`group_report.md`](report/team/group_report.md).
- Bảng phân công và các ghi chú được cả nhóm xác nhận khi hợp nhất repo.

**Điều mình học được từ phần nhóm:**

Việc chọn vấn đề cần dựa vào actor, quy trình và bằng chứng thay vì chỉ nhìn tính hấp dẫn của công nghệ. Một mô hình phát hiện động vật không tự động phát hiện được hành vi vi phạm; vì thế cần thiết kế nơi AI cảnh báo, con người kiểm chứng và bổ sung dữ liệu thật trước khi kết luận khả thi.

### Đặng Minh Thu - 2A202604009

**Phần việc phụ trách:**

- Nghiên cứu công cụ, giải pháp Computer Vision hiện có cho CP4.
- Phân tích quy trình trước/sau và các điểm nghẽn trong CP5.

**Đóng góp cụ thể:**

- Chuẩn bị ba Problem Cards gồm sự cố thú cưng, hỗ trợ ghi chú/hỏi đáp lớp học và phân loại yêu cầu đa kênh.
- Nghiên cứu Frigate NVR, AXIS Object Analytics và NVIDIA DeepStream; phân tích chức năng sẵn có, hạn chế khi phát hiện hành vi và khoảng trống cần thử nghiệm.
- Phác thảo quy trình As-Is từ tiếp nhận phản ánh, xác định camera, tìm video và xác minh; đề xuất To-Be sử dụng Rule, AI và bước nhân viên BQL kiểm tra.
- Làm rõ các thách thức về chất lượng CCTV, khả năng liên kết dữ liệu, sai số của AI và nhu cầu người kiểm tra trước khi xử lý.
- Đề xuất tiêu chí đo hiệu quả, nhưng các chỉ số thời gian thực tế vẫn cần baseline được kiểm chứng.

**Bằng chứng:**

- [Báo cáo cá nhân của Thu](report/individual/2A202604009_DangMinhThu.md), đặc biệt phần CP5.
- Mục 3.3 và mục 4 trong [`group_report.md`](report/team/group_report.md) (đã được cập nhật theo phạm vi cuối cùng).

**Điều mình học được từ phần nhóm:**

Cần phân biệt object detection với action/event detection và kiểm tra rủi ro khi AI kết luận sai. Công nghệ sẵn có có thể làm phần nền tảng, nhưng chất lượng dữ liệu và bước xác minh của con người vẫn quyết định giải pháp có hữu ích trong vận hành thực tế hay không.

### LeTheAnh-2A202603983
**Phần việc phụ trách:**
- CP6 — Xây dựng Problem Statement v1 và các tiêu chí đánh giá (mục 7 của báo cáo nhóm).
- CP6 — Phân tích rủi ro và đề xuất quyết định Go / Not Yet / No-Go (mục 8 của báo cáo nhóm).
- Thuyết trình đại diện nhóm MALTO trong buổi lab.
**Đóng góp cụ thể (mình đã làm gì, ra sản phẩm gì):**
- Tham gia xây dựng Problem Statement v1 cho bài toán quản lý và xác minh sự cố liên quan đến thú cưng tại khu chung cư.
- Phân tích Actor, quy trình hiện tại, bottleneck, impact, success metric và boundary của giải pháp.
- Làm rõ vai trò hỗ trợ của Computer Vision và trách nhiệm kiểm tra, xác minh của nhân viên an ninh trước khi thực hiện hành động.
- Xây dựng các tiêu chí đánh giá hiệu quả giải pháp, bao gồm chất lượng nhận diện, mức độ bỏ sót hoặc cảnh báo sai, và khả năng vận hành.
- Phân tích bốn nhóm rủi ro: Value, Usability, Feasibility và Viability.
- Đề xuất quyết định Not Yet đối với triển khai toàn diện, đồng thời xem xét thử nghiệm pilot giới hạn trước khi mở rộng.
- Đảm nhận nhiệm vụ thuyết trình, đại diện nhóm MALTO trình bày kết quả làm việc trong buổi lab.
**Bằng chứng (phần nào trong group_report.md, file nào trong report/assets/, commit nào):**
- report/team/group_report.md — mục 7: Problem Statement v1 và tiêu chí đánh giá.
- report/team/group_report.md — mục 8: Phân tích rủi ro và quyết định cuối.
- Vai trò thuyết trình trong buổi lab: có thể đối chiếu với các thành viên nhóm hoặc Lab Coach.
- Git commit: `3e16865`, `dd4d254` (thêm mục 7–8 vào báo cáo nhóm), `04ac42e` (báo cáo cá nhân).

**Điều mình học được từ phần nhóm:**

**Về AI và hiệu suất làm việc:** Qua buổi lab, mình nhận thấy AI thực sự rất quan trọng khi phải xử lý nhiều nhiệm vụ trong thời gian ngắn. AI có thể hỗ trợ tổng hợp thông tin, phân tích vấn đề, xây dựng cấu trúc báo cáo và phản biện ý tưởng với tốc độ rất nhanh. Tuy nhiên, tốc độ suy nghĩ, thảo luận và ra quyết định của con người không phải lúc nào cũng theo kịp tốc độ xử lý của AI. Điều này khiến mình nhận ra rằng sử dụng AI hiệu quả không chỉ phụ thuộc vào công cụ, mà còn phụ thuộc vào khả năng phối hợp và tổ chức công việc của cả nhóm.
**Về teamwork và điều phối thảo luận:** Mình nhận thấy việc tạo không khí thảo luận tích cực, khuyến khích các thành viên tham gia và phân chia nhiệm vụ phù hợp với thế mạnh của từng người là rất quan trọng. Đặc biệt trong một buổi lab có nhiều checkpoint và thời gian giới hạn, người điều phối cần giúp nhóm tập trung vào các quyết định quan trọng, tránh dành quá nhiều thời gian cho những vấn đề nhỏ. Khả năng kết nối các thành viên và tạo sự thoải mái khi trao đổi cũng ảnh hưởng trực tiếp đến hiệu quả làm việc nhóm.
**Về khả năng giao tiếp bằng tiếng Việt:** Mặc dù mình có nền tảng tiếng Trung và tiếng Anh tương đối tốt, buổi lab khiến mình nhận ra rằng những lợi thế này không thể bù đắp hoàn toàn cho hạn chế về tiếng Việt, đặc biệt khi cần thảo luận nhanh, trình bày ý tưởng và diễn đạt các khái niệm chuyên môn. Vì vậy, mình đặt mục tiêu trong hai tuần tới sẽ tăng cường đọc tài liệu tiếng Việt, đặc biệt là các nội dung về AI, công nghệ và quản lý sản phẩm, đồng thời luyện cách diễn đạt và thuyết trình để cải thiện khả năng giao tiếp trong môi trường học tập và làm việc nhóm.
**Về kiến thức AI cần bổ sung:** Mình đã có một số nền tảng về phân tích nghiệp vụ (Business Analysis), xác định vấn đề và xây dựng quy trình, nhưng nhận thấy bản thân vẫn còn thiếu kiến thức chuyên sâu về cách đánh giá chất lượng hệ thống AI. Những nội dung mình cần tiếp tục học bao gồm Precision, Recall, False Positive, False Negative, cách thiết kế bộ dữ liệu đánh giá (evaluation dataset), cách xác định baseline và target, cũng như cách đánh giá hiệu quả thực tế của AI sau khi đưa vào quy trình vận hành.
**Về việc lựa chọn giải pháp AI:** Một vấn đề mà mình muốn hiểu sâu hơn là khi nào nên sử dụng Rule-based System, Workflow có AI hỗ trợ hoặc AI Agent. Mình cần học cách đánh giá liệu AI có thực sự tạo ra giá trị vượt trội so với một quy trình đơn giản hơn hay không, đồng thời hiểu rõ các rủi ro khi AI đưa ra kết quả sai và vai trò của con người trong quá trình kiểm tra, xác minh.
**Định hướng cải thiện:** Trong những buổi lab tiếp theo, mình muốn cải thiện đồng thời ba năng lực: kiến thức kỹ thuật AI và phương pháp đánh giá hệ thống, khả năng tổ chức thảo luận nhóm, và khả năng sử dụng tiếng Việt trong môi trường chuyên môn. Mục tiêu không chỉ là hoàn thành các checkpoint đúng thời hạn mà còn thực sự hiểu được những quyết định kỹ thuật và sản phẩm mà nhóm đưa ra.
