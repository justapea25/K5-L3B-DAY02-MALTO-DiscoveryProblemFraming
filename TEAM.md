# Team

> Điền file này trên repo chung do nhóm trưởng fork. Nhóm điền phần **Thông tin nhóm** và **Thành viên**. Mỗi người tự điền phần của mình trong **Cá nhân**. Không copy file này sang repo khác.

## Thông tin nhóm

- Tên nhóm: MALTO
- Candidate problem nhóm chọn (1 câu): Hệ thống phát hiện sự cố thú cưng trong khu chung cư
- Quyết định cuối (Go / Not Yet / No-Go): Not Yet cho triển khai thương mại; Go cho pilot nhỏ

## Thành viên

| STT | Họ và tên      | MSSV        | Vai trò trong nhóm             | Tài khoản GitHub |
| --: | ----------------- | ----------- | -------------------------------- | ------------------ |
|   1 | Đậu Hoàng Minh    | 2A202604011 | Nhóm Trưởng, Thiết Kế Slide      | justapea25         |
|   2 | Lê Thế Anh        | 2A202603983 | CP6 (mục 7–8), thuyết trình      | LETHESHIYING       |
|   3 |                   |             |                                  |                    |
|   4 |                   |             |                                  |                    |

Không ghi email hay số điện thoại vào bảng này, vì repo có thể để public.

Gợi ý vai trò (một người có thể giữ nhiều vai): điều phối thời gian, ghi chép, người phản biện chính, phụ trách kiểm chứng (phỏng vấn/survey), phụ trách research, vẽ quy trình, viết Problem Statement.

## Phân công theo checkpoint

| Checkpoint                                    | Người chính | Người hỗ trợ | Sản phẩm                                      |
| --------------------------------------------- | -------------- | ---------------- | ----------------------------------------------- |
| CP3 — Hội tụ nhóm                         |                |                  | Cluster, cây OST, bảng chấm điểm           |
| CP4 — Kiểm chứng                           |                |                  | Assumption map, snapshot hoặc survey           |
| CP4 — Research                               |                |                  | Bảng research có link                         |
| CP5 — Quy trình trước/sau                 |                |                  | Quy trình + bảng before/after                 |
| CP5 — Problem Statement v0                   |                |                  | Problem Statement v0                            |
| CP6 — Mức can thiệp + Problem Statement v1 | Minh           | Thế Anh         | Ma trận, AI Canvas, eval, Problem Statement v1 |
| CP6 — Quyết định                          | Thế Anh       | Minh             | 4 rủi ro + Go/Not Yet/No-Go                    |

## Cá nhân

Mỗi thành viên thêm một mục theo mẫu dưới đây, tiêu đề là `HoVaTen-MSSV`.

### Đậu Hoàng Minh - 2A202604011

**Phần việc phụ trách:**

* Mục 6 – Mức can thiệp AI (ma trận độ mơ hồ × độ phức tạp, so sánh 4 mức, AI Canvas, 2 câu hỏi Google PAIR)
* Mục 9 – Hạn chế và hướng tiếp theo
* Slide pitch (7 trang), gồm quy trình hiện tại và quy trình 3 bước
* Phân tích các ý kiến problem, đưa ra giải pháp kĩ thuật cho problem đề ra.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

* Ở giai đoạn chọn đề tài: pitch card tổng hợp sau cuộc họp, phản biện card của các bạn khác
* Đề xuất tách bài toán truy vết sự cố thú cưng thành 3 bước: (1) phát hiện sự kiện, (2) xác nhận thú cưng, (3) truy vết căn hộ, thay vì cho AI nhận diện thẳng căn hộ từ video. Nhờ đó nhóm thấy bottleneck nằm ở bước tìm đoạn video và thu hẹp phạm vi AI.
* Viết mục 6: xếp bài vào ô “độ mơ hồ thấp × độ phức tạp cao”, lập luận vì sao No AI và Rule không đủ, vì sao không cần Agent, và chọn Workflow. Hoàn thành AI Canvas và phân tích báo nhầm/bỏ sót theo từng bước.
* Viết mục 9: liệt kê hạn chế về bằng chứng, dữ liệu camera, quyền riêng tư, phạm vi giải pháp, đề xuất hướng tiếp theo
* Làm slide pitch 7 trang cho bài thuyết trình

**Bằng chứng**

- Mục 6 và Mục 9 trong file `group_report.md`
- File `cp5-workflow-current.png` trong `report/assets/` (quy trình hiện tại, chụp từ slide pitch)
- Commit 77c2f95712f4ea86e5b8e01c0403c0f3204b438e thêm mục 6, mục 9 vào file group report

**Điều mình học được từ phần nhóm:**

Mình học được rằng chọn mức AI phải đi từ mức đơn giản nhất và chỉ áp dụng khi cần thiết. Lúc đầu cả nhóm có suy nghĩ AI làm hết cho cả quy trình nhận diện thú cưng vi phạm, nhưng khi vẽ lại quy trình thì thấy chỉ cần AI ở đúng bước tìm video, còn quyết định căn hộ nào vi phạm phải để con người làm. Mình cũng học được là cùng một lỗi của AI có thể rẻ ở bước này nhưng rất đắt ở bước khác: bỏ sót đoạn video thì chỉ tốn công, nhưng nêu nhầm căn hộ thì gây mâu thuẫn. Cuối cùng, việc card của mình bị loại vì đã có nhiều tool giải quyết giúp mình hiểu một problem tốt không chỉ cần pain thật mà còn phải có khoảng trống thật.


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
- Git commit: [BỔ SUNG COMMIT HASH NẾU CẦN].

**Điều mình học được từ phần nhóm:**

**Về AI và hiệu suất làm việc:** Qua buổi lab, mình nhận thấy AI thực sự rất quan trọng khi phải xử lý nhiều nhiệm vụ trong thời gian ngắn. AI có thể hỗ trợ tổng hợp thông tin, phân tích vấn đề, xây dựng cấu trúc báo cáo và phản biện ý tưởng với tốc độ rất nhanh. Tuy nhiên, tốc độ suy nghĩ, thảo luận và ra quyết định của con người không phải lúc nào cũng theo kịp tốc độ xử lý của AI. Điều này khiến mình nhận ra rằng sử dụng AI hiệu quả không chỉ phụ thuộc vào công cụ, mà còn phụ thuộc vào khả năng phối hợp và tổ chức công việc của cả nhóm.
**Về teamwork và điều phối thảo luận:** Mình nhận thấy việc tạo không khí thảo luận tích cực, khuyến khích các thành viên tham gia và phân chia nhiệm vụ phù hợp với thế mạnh của từng người là rất quan trọng. Đặc biệt trong một buổi lab có nhiều checkpoint và thời gian giới hạn, người điều phối cần giúp nhóm tập trung vào các quyết định quan trọng, tránh dành quá nhiều thời gian cho những vấn đề nhỏ. Khả năng kết nối các thành viên và tạo sự thoải mái khi trao đổi cũng ảnh hưởng trực tiếp đến hiệu quả làm việc nhóm.
**Về khả năng giao tiếp bằng tiếng Việt:** Mặc dù mình có nền tảng tiếng Trung và tiếng Anh tương đối tốt, buổi lab khiến mình nhận ra rằng những lợi thế này không thể bù đắp hoàn toàn cho hạn chế về tiếng Việt, đặc biệt khi cần thảo luận nhanh, trình bày ý tưởng và diễn đạt các khái niệm chuyên môn. Vì vậy, mình đặt mục tiêu trong hai tuần tới sẽ tăng cường đọc tài liệu tiếng Việt, đặc biệt là các nội dung về AI, công nghệ và quản lý sản phẩm, đồng thời luyện cách diễn đạt và thuyết trình để cải thiện khả năng giao tiếp trong môi trường học tập và làm việc nhóm.
**Về kiến thức AI cần bổ sung:** Mình đã có một số nền tảng về phân tích nghiệp vụ (Business Analysis), xác định vấn đề và xây dựng quy trình, nhưng nhận thấy bản thân vẫn còn thiếu kiến thức chuyên sâu về cách đánh giá chất lượng hệ thống AI. Những nội dung mình cần tiếp tục học bao gồm Precision, Recall, False Positive, False Negative, cách thiết kế bộ dữ liệu đánh giá (evaluation dataset), cách xác định baseline và target, cũng như cách đánh giá hiệu quả thực tế của AI sau khi đưa vào quy trình vận hành.
**Về việc lựa chọn giải pháp AI:** Một vấn đề mà mình muốn hiểu sâu hơn là khi nào nên sử dụng Rule-based System, Workflow có AI hỗ trợ hoặc AI Agent. Mình cần học cách đánh giá liệu AI có thực sự tạo ra giá trị vượt trội so với một quy trình đơn giản hơn hay không, đồng thời hiểu rõ các rủi ro khi AI đưa ra kết quả sai và vai trò của con người trong quá trình kiểm tra, xác minh.
**Định hướng cải thiện:** Trong những buổi lab tiếp theo, mình muốn cải thiện đồng thời ba năng lực: kiến thức kỹ thuật AI và phương pháp đánh giá hệ thống, khả năng tổ chức thảo luận nhóm, và khả năng sử dụng tiếng Việt trong môi trường chuyên môn. Mục tiêu không chỉ là hoàn thành các checkpoint đúng thời hạn mà còn thực sự hiểu được những quyết định kỹ thuật và sản phẩm mà nhóm đưa ra.
