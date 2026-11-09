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
| 2 | Nguyễn Xuân Khánh Linh | 2A202603801 | Điều phối thảo luận CP3–CP4; lập bảng tiêu chí chọn candidate; Assumption Map và hỗ trợ research | Chưa cung cấp |
| 3 | Đặng Minh Thu | 2A202604009 | Research công nghệ; phân tích quy trình trước/sau (CP5) | Chưa cung cấp |
| 4 | Lê Thế Anh | 2A202603983 | Đề xuất bài toán thú cưng; Problem Statement v1, tiêu chí đánh giá và quyết định CP6 | Chưa cung cấp |

*Không công khai email/số điện thoại trong bảng này. Vai trò phản ánh đóng góp được mô tả trong tài liệu hiện có; nhóm cần xác nhận nếu có thay đổi phân công.*

## Phân công theo checkpoint

| Checkpoint | Người chính | Người hỗ trợ | Sản phẩm |
|---|---|---|---|
| CP3 — Hội tụ nhóm | Nguyễn Xuân Khánh Linh | Đậu Hoàng Minh; các thành viên góp candidate | Cluster, cây OST, bảng chấm theo 7 tiêu chí, lý do chọn |
| CP4 — Kiểm chứng | Nguyễn Xuân Khánh Linh | Lê Thế Anh (cung cấp phản ánh cư dân) | Assumption Map, câu hỏi phỏng vấn, snapshot / survey khi có dữ liệu |
| CP4 — Research | Đặng Minh Thu | Nguyễn Xuân Khánh Linh; Đậu Hoàng Minh rà nội dung thuyết trình | Bảng research Frigate, AXIS, NVIDIA có nguồn và khoảng trống |
| CP5 — Quy trình trước/sau | Đặng Minh Thu | Đậu Hoàng Minh (slide quy trình) | Workflow As-Is/To-Be và so sánh before/after |
| CP5 — Problem Statement v0 | **Cần nhóm xác nhận người chính** | Đặng Minh Thu; Lê Thế Anh | Problem Statement v0 |
| CP6 — Mức can thiệp + Problem Statement v1 | Đậu Hoàng Minh | Lê Thế Anh | Ma trận, AI Canvas, PAIR, evaluation, Problem Statement v1 |
| CP6 — Quyết định | Lê Thế Anh | Đậu Hoàng Minh | Bốn rủi ro + Go / Not Yet / No-Go |

> **Lưu ý về các phiên bản:** Trong các bản cá nhân giai đoạn đầu, giải pháp từng bao gồm truy vết thú cưng và xác định căn hộ. Báo cáo nhóm phiên bản hiện tại đã **thu hẹp thành phát hiện/cảnh báo sớm và con người xác minh**. Những phần đóng góp ghi nhận ý tưởng cũ là lịch sử phát triển phương án, không phải tính năng nhóm cam kết triển khai cuối cùng.

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
- Viết mục 6: xếp bài vào ô “độ mơ hồ thấp × độ phức tạp cao”, lập luận vì sao No AI và Rule chưa đủ, vì sao không cần Agent, và chọn Workflow. Hoàn thành AI Canvas và phân tích báo nhầm/bỏ sót theo từng bước.
- Viết mục 9: liệt kê hạn chế về bằng chứng, dữ liệu camera, quyền riêng tư, phạm vi giải pháp, đề xuất hướng tiếp theo.
- Làm slide pitch 7 trang cho bài thuyết trình.

**Bằng chứng:**

- Mục 6 và Mục 9 trong file `report/team/group_report.md` (đã có điều chỉnh theo phương án cuối).
- File `report/assets/cp5-workflow-current.png` nếu nhóm đã đưa ảnh lên repo (quy trình hiện tại từ slide pitch).
- Commit `77c2f95712f4ea86e5b8e01c0403c0f3204b438e` thêm mục 6, mục 9 vào báo cáo nhóm (theo thông tin Minh cung cấp).
- [Báo cáo cá nhân](report/individual/2A202604011_DauHoangMinh.md).

**Điều mình học được từ phần nhóm:**

Mình học được rằng chọn mức AI phải đi từ mức đơn giản nhất và chỉ áp dụng khi cần thiết. Lúc đầu cả nhóm có suy nghĩ AI làm hết cho cả quy trình nhận diện thú cưng vi phạm, nhưng khi vẽ lại quy trình thì thấy chỉ cần AI ở đúng bước phù hợp, còn quyết định xử lý phải để con người làm. Mình cũng học được là cùng một lỗi của AI có thể rẻ ở bước này nhưng rất đắt ở bước khác: bỏ sót đoạn video thì tốn công, nhưng nêu nhầm căn hộ có thể gây mâu thuẫn. Cuối cùng, việc card của mình bị loại vì đã có nhiều tool giải quyết giúp mình hiểu một problem tốt không chỉ cần pain thật mà còn phải có khoảng trống thật.

### Nguyễn Xuân Khánh Linh - 2A202603801

**Phần việc phụ trách:**

- Điều phối công việc và thảo luận CP3–CP4.
- Lập bảng tiêu chí đánh giá candidate theo bảy yếu tố của rubric CP3 và hỗ trợ nhóm chọn vấn đề.
- Chuẩn bị Assumption Map, bộ câu hỏi kiểm chứng theo The Mom Test; tổng hợp research và lý do thu hẹp problem ở CP4.

**Đóng góp cụ thể:**

- Chuẩn bị ba Problem Cards cá nhân: creative chờ test, thiết lập remote key lặp lại và hỗ trợ sửa IELTS Writing. Đưa các candidate này vào quá trình cân nhắc; **lượt pitch trực tiếp cụ thể cần người viết xác nhận**.
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
- Làm rõ các thách thức về chất lượng CCTV, khả năng liên kết dữ liệu, sai số của AI và nhu cầu người kiểm tra trước khi xử lý. **Phạm vi truy vết trong bản đầu đã được nhóm bỏ khỏi giải pháp cuối.**
- Đề xuất tiêu chí đo hiệu quả, nhưng các chỉ số thời gian thực tế vẫn cần baseline được kiểm chứng.

**Bằng chứng:**

- [Báo cáo cá nhân của Thu](report/individual/2A202604009_DangMinhThu.md), đặc biệt phần CP5.
- Mục 3.3 và mục 4 trong [`group_report.md`](report/team/group_report.md) (đã được cập nhật theo phạm vi cuối cùng).

**Điều mình học được từ phần nhóm:**

Cần phân biệt object detection với action/event detection và kiểm tra rủi ro khi AI kết luận sai. Công nghệ sẵn có có thể làm phần nền tảng, nhưng chất lượng dữ liệu và bước xác minh của con người vẫn quyết định giải pháp có hữu ích trong vận hành thực tế hay không.

### Lê Thế Anh - 2A202603983

**Phần việc phụ trách:**

- Đề xuất bài toán thú cưng và bổ sung tín hiệu ban đầu từ lời kể cư dân.
- Phụ trách nội dung Problem Statement v1, tiêu chí đánh giá và phần quyết định CP6.

**Đóng góp cụ thể:**

- Đưa vào CP1 tình huống cư dân phản ánh nuôi thú cưng trái nội quy, gây ồn, phóng uế khu vực chung; đây là **lời kể từ một cư dân**, không phải số liệu sự cố đã thống kê.
- Chuẩn bị Problem Card về sự cố thú cưng, đồng thời so sánh với các vấn đề căn tin VinUni và xe buýt đông khách.
- Viết bản nháp `Problem Statement v1` (actor, workflow, bottleneck, impact, metric, boundary), bộ năm tiêu chí eval và đề xuất Human-in-the-loop.
- Chuẩn bị phần bốn rủi ro Value, Usability, Feasibility, Viability và phương án **Not Yet** cho triển khai rộng, **Go có điều kiện** cho pilot nhỏ.
- Nhận diện sự khác biệt giữa phát hiện đối tượng và xác định vi phạm; lưu ý việc suy ra căn hộ từ CCTV là rủi ro. Những nội dung theo dõi liên camera trong bản nháp cũ không nằm trong phạm vi cuối cùng.

**Bằng chứng:**

- [Báo cáo cá nhân của Thế Anh](report/individual/2A202603983_LeTheAnh.md).
- Mục 7–8 trong [`group_report.md`](report/team/group_report.md) (đã chỉnh về phát hiện/cảnh báo).
- Nội dung CP6 được Thế Anh mô tả đã chuẩn bị trên nhánh `theanh`; nhóm cần kiểm tra commit cụ thể khi hợp nhất.

**Điều mình học được từ phần nhóm:**

Một vấn đề có thể ảnh hưởng tới cư dân nhưng phải chứng minh tần suất, bottleneck và thời gian xử lý bằng dữ liệu thay vì giả định. Khi thiết kế ứng dụng AI từ CCTV cần giới hạn phạm vi, có con người xác minh và không để hệ thống tự quy kết trách nhiệm.
