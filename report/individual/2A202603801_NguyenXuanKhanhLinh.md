# Báo cáo cá nhân — 2A202603801_NguyenXuanKhanhLinh

## 1. Thông tin học viên

- Họ tên: **Nguyễn Xuân Khánh Linh**
- MSSV: **2A202603801**
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: **MALTO — L3B**
- Link repo nhóm: https://github.com/justapea25/K5-L3B-DAY02-MALTO-DiscoveryProblemFraming/

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Tốn thời gian | Khi chạy nhiều campaign quảng cáo cùng lúc, tôi muốn phát hiện kịp thời khi CPI, ROAS hoặc spend vượt ngưỡng cần xử lý, để điều chỉnh trước khi ngân sách tiếp tục bị sử dụng kém hiệu quả. | UA team | Ước tính cá nhân: hơn **2 giờ/ngày** để theo dõi campaign (hơn **10 giờ/tuần làm việc**). Chưa có log đo thời gian hay ngân sách phát sinh do phát hiện chậm. |
| 2 | Tốn thời gian / Pain từ người khác | Khi creative mới được bàn giao, tôi muốn biết creative nào chưa được đưa vào campaign test và lý do đang chờ, để hạn chế bỏ sót creative đủ điều kiện và tránh trì hoãn không cần thiết. | UA team; Creative team | **Creative Hub (Sonat BI), task tạo tháng 10/2026, tính đến 08/11:** 109/235 task (46,4%) còn `waiting`; 109 task chờ trên 7 ngày, 78 task chờ trên 14 ngày; lâu nhất 37 ngày. Chưa xác minh những task này có thực sự quá hạn hay bị bỏ sót không. |
| 3 | Lặp lại | Khi thiết lập ads scenario cho một game, tôi muốn giảm các thao tác gán remote key và nhập giá trị cấu hình trùng lặp giữa những game có yêu cầu tương tự, để tiết kiệm thời gian và giảm lỗi setup. | Monetization (MO) team | MO Remote Setup (Sonat BI), 08/11/2026: 256 campaign/154 game; 2.592 lượt gán key (trung vị 7, cao nhất 57 key/campaign); 1.728 giá trị key trong 622 ad group; 41 bộ key dùng cho ít nhất 2 game, bộ phổ biến nhất ở 12 game. Chưa đo thời gian và mức độ setup thủ công. |
| 4 | Lặp lại / Tốn thời gian | Khi chấm IELTS Writing và đã ghi nhận xét về một câu, tôi muốn nhanh chóng có phương án sửa đúng với comment và phong cách phản hồi của mình, để giảm thời gian viết câu sửa mẫu mà vẫn giữ chất lượng và tính nhất quán. | Giáo viên IELTS Writing; học sinh nhận feedback | Chưa có số đo thực tế: cần ghi thời gian chấm/bài, thời gian viết câu sửa và số câu cần sửa. |
| 5 | Cần đọc, tổng hợp nhiều thông tin / Tốn thời gian | Khi tham gia bài giảng có nhiều kiến thức mới, tôi muốn ghi chú theo cấu trúc rõ ràng, bổ sung và phân loại ghi chú cá nhân (định nghĩa, ví dụ, công thức...), đồng thời được giải đáp thắc mắc riêng tư ngay trong buổi học, để không mất mạch bài và dễ ôn tập sau lớp. | Sinh viên, người tham gia khóa học | Chưa có số đo: cần khảo sát thời gian tổ chức lại ghi chú, số thắc mắc chưa được hỏi và mức độ đầy đủ của notes. |

**Nếu có dùng AI để gợi ý thêm:** Tôi sử dụng AI để rà lại cách diễn đạt Job Story và phân biệt vấn đề với giải pháp. Tôi giữ những ý có bối cảnh công việc hoặc học tập cụ thể; không đưa các ý tưởng giải pháp quá rộng như một agent tự quản lý toàn bộ quy trình vào danh sách.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao đưa vào Top 3 | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | **#2 — Creative waiting** | Có dữ liệu backlog theo task; actor rõ; có thể kiểm chứng thời gian từ bàn giao đến test. | waiting có phải quá hạn/bỏ sót? Vì sao task chờ? |
| 2 | **#3 — Remote key setup** | Có log quy mô thao tác và cấu hình lặp lại; dễ so sánh template/rule với AI. | Setup hiện có thủ công không? Value của các bộ key có đủ giống để tái sử dụng không? |
| 3 | **#4 — IELTS Writing feedback** | Nhiệm vụ hiểu comment và tái diễn đạt theo phong cách là điểm AI có khả năng giúp trực tiếp. | Mất bao lâu khi viết câu sửa? Dữ liệu chấm cũ có được phép dùng và đủ nhất quán không? |

### Problem Card #1 — Creative chờ test

| Trường | Nội dung |
|---|---|
| **Job Story** | Khi creative đã được bàn giao, UA muốn biết creative nào chưa được test và vì sao, để giảm bỏ sót creative đủ điều kiện và rút ngắn thời gian chờ không cần thiết. |
| **Actor** | UA nhận bàn giao và chạy test; Creative team theo dõi đầu ra. |
| **Thời điểm / bối cảnh** | Khi creative đã hoàn thành và được cập nhật lên Creative Hub / quy trình bàn giao. |
| **Quy trình hiện tại (giả thuyết)** | 1. Creative hoàn thiện → 2. Review/bàn giao → 3. Task chuyển trạng thái waiting → 4. UA xem danh sách và xếp ưu tiên → 5. Tạo campaign test → 6. Cập nhật trạng thái/kết quả. |
| **Bottleneck giả định** | **Bước 3–4:** creative chờ giữa bàn giao và quyết định được đưa lên test. **Chưa chứng minh** đây là lỗi theo dõi, thiếu ngân sách hay chủ động hoãn. |
| **Impact** | Có nguy cơ lỡ cơ hội kiểm thử creative, phát sinh backlog và chậm feedback giữa team. **Chưa định lượng doanh thu/cơ hội bị mất.** |
| **Evidence** | Snapshot 08/11/2026: **109/235** task tháng 10 còn waiting; **78** đã chờ trên 14 ngày; lâu nhất **37 ngày**. Đây là thời gian chờ, **không phải** bằng chứng mọi task đã quá hạn. |
| **Success metric** | Thời gian **ready-for-test → first-test**: **[X ngày] → [Y ngày]**, tách theo lý do chờ; tỷ lệ creative đủ điều kiện được test đúng SLA **[X%] → [Y%]**. Baseline chưa có. |
| **No-AI Alternative** | Dashboard backlog theo owner/tuổi task, SLA, rule nhắc quá hạn, bắt buộc ghi lý do waiting. |
| **Giả thuyết AI** | Khi lý do chờ nằm trong trao đổi phi cấu trúc, LLM có thể tóm tắt status, nhóm nguyên nhân và hỗ trợ UA ưu tiên danh sách cần kiểm tra; con người quyết định test. |
| **Cảm nhận nhanh** | **Rule/Workflow trước**; AI chỉ cần khi thông tin phân tán/khó chuẩn hóa. |

**Quy trình hiện tại (cần đo thời gian thực tế):**

```text
[1. Creative hoàn thiện: ___ phút/giờ]
    → [2. Review + bàn giao: ___]
    → [3. Cập nhật task waiting: ___]
    → [4. UA kiểm tra + xếp lịch test: ___]  ← BOTTLENECK CẦN XÁC MINH
    → [5. Tạo campaign test: ___]
    → [6. Cập nhật trạng thái + kết quả: ___]
```

*Thời gian chờ task và thời gian thao tác của nhân viên được đo riêng.*

### Problem Card #2 — Thiết lập remote key lặp lại

| Trường | Nội dung |
|---|---|
| **Job Story** | Khi thiết lập ads scenario cho một game, MO muốn giảm việc cấu hình key/value trùng lặp, để tiết kiệm thời gian và giảm lỗi setup. |
| **Actor** | Nhân viên Monetization (MO) setup ads scenario. |
| **Thời điểm / bối cảnh** | Khi tạo/chỉnh sửa campaign hoặc ad group cho game có cấu hình tương tự game đã triển khai. |
| **Quy trình hiện tại (giả thuyết)** | 1. Nhận yêu cầu setup → 2. Tìm kịch bản tương tự → 3. Chọn/gán key → 4. Nhập value → 5. Kiểm tra cấu hình → 6. Lưu/áp dụng. |
| **Bottleneck giả định** | **Bước 3–4:** gán key và điền value có thể lặp lại. **Chưa xác nhận** thao tác có thủ công hay chưa có chức năng sao chép/template. |
| **Impact** | Tốn công thiết lập, nguy cơ nhập sai key/value và phải sửa. Chưa đo phút/campaign hoặc lỗi setup. |
| **Evidence** | MO Remote Setup, 08/11/2026: **256 campaign / 154 game**, **2.592 lượt gán key**, **1.728 value / 622 ad group**, **41 bộ key** dùng ở ≥2 game (bộ phổ biến nhất ở 12 game). Giống bộ key **không đảm bảo value cũng giống nhau**. |
| **Success metric** | Thời gian setup mỗi campaign **[X phút] → [Y phút]**; số thao tác gán key thủ công **[X] → [Y]**; tỷ lệ lỗi cấu hình **[X%] → [Y%]**. |
| **No-AI Alternative** | Template/preset có version, sao chép kịch bản, rule kiểm tra key/value bắt buộc. |
| **Giả thuyết AI** | Chỉ khi yêu cầu cấu hình đầu vào là mô tả tự nhiên, LLM mới có thể hỗ trợ đề xuất preset phù hợp rồi để MO duyệt. Không để AI tự áp dụng cấu hình nhạy cảm. |
| **Cảm nhận nhanh** | **No AI / Rule là ứng viên mạnh hơn AI** cho phần lớn bước lặp lại. |

**Quy trình nháp:**

```text
[1. Nhận yêu cầu: ___ phút]
    → [2. Tra cấu hình tương tự: ___ phút]
    → [3. Chọn và gán remote key: ___ phút]  ← BOTTLENECK GIẢ ĐỊNH
    → [4. Nhập value / chỉnh riêng: ___ phút]
    → [5. Review cấu hình: ___ phút]
    → [6. Lưu và áp dụng: ___ phút]
```

### Problem Card #3 — Viết câu sửa IELTS Writing

| Trường | Nội dung |
|---|---|
| **Job Story** | Khi đã nhận xét một câu trong IELTS Writing, giáo viên muốn có phương án sửa sát comment và phong cách phản hồi của mình, để giảm thời gian viết câu sửa mà vẫn giữ chất lượng. |
| **Actor** | Giáo viên chấm IELTS Writing; học sinh nhận feedback. |
| **Thời điểm / bối cảnh** | Sau khi giáo viên đọc câu và ghi comment về lỗi/ngữ nghĩa/phong cách diễn đạt. |
| **Quy trình hiện tại (giả thuyết)** | 1. Đọc bài → 2. Xác định vấn đề trong câu → 3. Ghi comment → 4. Tự nghĩ/viết câu sửa → 5. Soát nghĩa và phong cách → 6. Gửi feedback. |
| **Bottleneck giả định** | **Bước 4 — Tự viết câu sửa mẫu** lặp lại cho nhiều câu/bài. Chưa đo thời gian riêng bước này. |
| **Impact** | Chiếm thời gian chấm, có nguy cơ thiếu nhất quán giữa nhiều bài nếu chấm với khối lượng lớn; impact cần đo. |
| **Evidence** | Có **Job Story từ trải nghiệm dạy IELTS**; **chưa có baseline định lượng**. Cần ghi giờ chấm tối thiểu một số bài và số câu thực sự cần sửa. |
| **Success metric** | Thời gian sửa một câu **[X giây] → [Y giây]**; thời gian chấm một bài **[X phút] → [Y phút]**; tỷ lệ đề xuất phù hợp comment, giữ ý gốc và được giáo viên chấp nhận. |
| **No-AI Alternative** | Bộ câu sửa mẫu, checklist lỗi phổ biến, rubric phản hồi cá nhân, text-expander. |
| **Giả thuyết AI** | **Workflow + LLM:** câu gốc + comment + style guide/ví dụ đã được phép sử dụng → AI đề xuất 1–2 câu sửa → giáo viên duyệt/chỉnh/từ chối. Không tự chấm band hay gửi feedback. |
| **Cảm nhận nhanh** | **Workflow + LLM** có tiềm năng vì bài toán cần hiểu ngữ nghĩa và ngữ cảnh. |

**Quy trình nháp:**

```text
[1. Đọc câu/đoạn: ___ giây]
    → [2. Xác định điểm cần sửa: ___ giây]
    → [3. Ghi comment: ___ giây]
    → [4. Soạn câu sửa mẫu: ___ giây]  ← BOTTLENECK GIẢ ĐỊNH
    → [5. Kiểm tra giữ ý gốc: ___ giây]
    → [6. Hoàn thiện feedback: ___ giây]
```

### Card muốn pitch nhất

- Card số: 2 
- Vì sao: Tôi ưu tiên bài toán này vì có bằng chứng thực tế từ Creative Hub: 109/235 task tạo trong tháng 10/2026 vẫn ở trạng thái waiting tính đến 08/11, trong đó 78 task đã chờ hơn 14 ngày. Actor và quy trình bàn giao giữa Creative và UA tương đối rõ, có thể kiểm chứng nguyên nhân chờ và đo thời gian từ lúc creative sẵn sàng đến khi được test. Tuy nhiên, cần xác định đâu là chờ có chủ đích, đâu là chậm xử lý trước khi đề xuất giải pháp AI.
- Câu hỏi muốn nhóm phản biện: 109 task waiting có thực sự phản ánh việc bỏ sót hoặc chậm test không? Nếu có, liệu rule-based tracking và cảnh báo quá hạn đã đủ giải quyết, hay AI có thể tạo thêm giá trị?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Creative waiting: task `waiting` chưa chắc bị bỏ sót hoặc quá hạn. | Đồng ý | Không coi backlog là số task bị bỏ quên; thêm yêu cầu xác minh lý do chờ và SLA. |
| Remote key: bộ key giống nhau không đảm bảo value giống nhau; template có thể đã đủ. | Đồng ý | Bổ sung phương án template/rule và yêu cầu đo thời gian setup, mức trùng lặp key/value. |
| IELTS feedback: câu sửa nhanh nhưng sai ý hoặc không khớp comment thì không cải thiện việc chấm. | Đồng ý | Bổ sung tiêu chí giữ ý gốc, khớp nhận xét và giáo viên duyệt trước khi dùng. |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

**Vai trò chính:** Tôi tham gia và điều phối công việc nhóm ở **CP3 (Hội tụ, chọn bài toán)** và **CP4 (Kiểm chứng, research)**.

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card (ý tưởng của tôi) | Tôi chuẩn bị 3 Problem Card cá nhân về creative chờ test, thiết lập remote key và hỗ trợ sửa IELTS Writing để đưa vào phần pitch. Bài toán đã trực tiếp trình bày: creative chờ test. | Cung cấp những phương án cá nhân để nhóm xem xét trong CP3. |
| Phản biện bài của bạn khác | Khi nghe các thành viên khác pitch, tôi đặt hai câu hỏi: **“Ứng dụng này chỉ sửa UI/UX à bạn?” và **“Ứng dụng này khác gì dùng ChatGPT để sửa CV?” | Yêu cầu làm rõ vấn đề thực sự được giải quyết và điểm khác biệt so với giải pháp sẵn có; giúp nhóm đánh giá candidate kỹ hơn.|
| Nhận phản biện || |
| Gom cluster / cây OST | Tôi tham gia tổng hợp các ý tưởng từ mảng game, IELTS, học tập và khu đô thị để phục vụ phần hội tụ candidate ở CP3. | Có dữ liệu đầu vào cho phần phân nhóm và shortlist; việc trực tiếp xây cây OST cần đối chiếu với phân công thực tế của nhóm. |
| Chọn candidate problem | Tôi lập bảng tiêu chí để đánh giá các candidate, dựa trên 7 yếu tố: actor rõ, workflow rõ, pain có bằng chứng, impact đo được, vừa sức lab, so sánh được 4 mức can thiệp và nhóm hiểu domain. Tôi sử dụng kết quả đánh giá để hỗ trợ nhóm chọn bài toán cảnh báo sự cố thú cưng. | Giúp nhóm lựa chọn có căn cứ, thay vì chỉ dựa vào mức độ hấp dẫn của giải pháp AI. |
| Kiểm chứng / research (CP4) | Tôi chuẩn bị Assumption Map, các câu hỏi phỏng vấn theo The Mom Test và nghiên cứu ba giải pháp **Frigate NVR, AXIS Object Analytics, NVIDIA DeepStream**. Tôi so sánh khả năng phát hiện đối tượng với khả năng nhận diện hành vi sự cố. | Hoàn thiện nội dung research CP4; xác định các giả định còn thiếu bằng chứng, nhất là độ trễ phát hiện, tính khả thi của CCTV và tỷ lệ cảnh báo sai. Chưa ghi nhận có phỏng vấn hoặc khảo sát thực tế. |
| Quy trình nhóm | Tôi điều phối quá trình làm việc và thảo luận của nhóm ở CP3–CP4, hỗ trợ kết nối phần chọn bài toán với phần kiểm chứng và research. | Giúp các nội dung đi theo một mạch: chọn candidate → kiểm chứng giả định → nghiên cứu giải pháp → điều chỉnh phạm vi. |
| Problem Statement / Problem Refinement | Tôi tham gia điều chỉnh hướng bài toán từ truy vết thú cưng, xác định căn hộ sang phát hiện dấu hiệu nghi vấn và cảnh báo để con người kiểm tra**; loại bỏ thất lạc, tập trung vào phóng uế, không rọ mõm tại khu vực có quy định và dấu hiệu gây thương tích. | Phạm vi cụ thể, phù hợp với cơ chế cảnh báo từ CCTV; nhân viên an ninh và BQL vẫn chịu trách nhiệm xác minh, xử lý. |
| Mức can thiệp AI | Tôi góp ý giới hạn AI ở phát hiện dấu hiệu nghi vấn và gửi cảnh báo, không tự kết luận vi phạm, xác định chủ sở hữu hoặc xử phạt. |  |
| Quyết định | Tôi đưa ra các điều kiện cần kiểm chứng trước khi triển khai như tần suất sự cố, chất lượng CCTV, khả năng phát hiện hành vi và số cảnh báo sai. | Cung cấp thông tin đầu vào để nhóm đánh giá Go / Not Yet / No-Go ở CP6 |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Rà cách viết Job Story, tách nhu cầu khỏi giải pháp. | Giúp diễn đạt ngắn gọn và đúng cấu trúc Khi – tôi muốn – để. | | Giữ lại số liệu nguồn, đánh dấu các giả định chưa xác minh. |
| CP2 Problem Card | Hỗ trợ sắp xếp ba Problem Card, phác thảo workflow và gợi ý cách đo. | Gợi ý phương án không dùng AI ở từng bài toán. | | |
| CP4 Research | Hỗ trợ tổng hợp và so sánh Frigate, AXIS Object Analytics và NVIDIA DeepStream cho bài toán cảnh báo sự cố thú cưng. | | | |
| CP5 Quy trình | | | | |
| CP5–6 Problem Statement | | | | |
| CP6 Mức can thiệp / quyết định | | | | |
| CP7 Reflection | | | | |

---

## 6. Reflection (CP7)

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

Khi so sánh những bài toán được đưa ra trong quá trình làm lab, tôi nhận ra một vấn đề có nhiều số liệu chưa chắc đã là vấn đề nên dùng AI. Ví dụ, việc creative bị tồn ở trạng thái waiting hoặc phải thiết lập remote key lặp lại có thể được cải thiện bằng quy trình, dashboard hoặc template. Ngược lại, bài toán cảnh báo sự cố thú cưng có cơ hội ứng dụng Computer Vision nhưng khó hơn về dữ liệu và khả năng nhận diện hành vi. Vì vậy, khi chọn bài toán, tôi cần xem đồng thời pain, bằng chứng, impact và tính khả thi chứ không chỉ chọn ý tưởng nghe hấp dẫn.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

Ở ý tưởng quản lý sự cố thú cưng, hướng giải pháp ban đầu khá rộng: phát hiện sự cố, truy vết thú cưng rồi xác định căn hộ liên quan. Cách tiếp cận này xuất phát từ những gì AI có thể làm, trong khi chưa xác minh được BQL thực sự vướng nhất ở bước nào. Khi phân tích lại, nhóm thu hẹp mục tiêu thành cảnh báo sớm các tình huống nghi vấn để an ninh kiểm tra. Phạm vi hiện tại là phóng uế, không rọ mõm ở khu vực có yêu cầu và dấu hiệu gây thương tích. Việc xác minh và xử lý vẫn do con người quyết định.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

Một điểm khiến tôi thay đổi cách nhìn là nhận xét rằng phát hiện được chó hoặc mèo trên camera không có nghĩa là đã nhận diện được hành vi vi phạm. Ban đầu tôi nghĩ có thể dùng một giải pháp Computer Vision chung cho các tình huống liên quan đến thú cưng. Sau khi xem xét kỹ hơn, tôi thấy từng hành vi cần dấu hiệu và dữ liệu đánh giá khác nhau; riêng việc không rọ mõm còn phụ thuộc góc quay và quy định của từng khu vực. Vì vậy, tôi đồng ý với hướng chỉ phát cảnh báo nghi vấn, đính kèm video để nhân viên xác minh, thay vì để AI tự kết luận.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

Điều đáng chú ý nhất từ research là công nghệ phát hiện đối tượng và gửi cảnh báo đã có trong những hệ thống như Frigate hay các nền tảng phân tích video. Nhóm không nhất thiết phải tự xây mọi thành phần từ đầu. Tuy nhiên, các công cụ này không chứng minh sẵn khả năng xác định chính xác hành vi phóng uế, không rọ mõm hoặc gây thương tích trong CCTV thực tế của khu đô thị. Hiện nhóm chưa có kết quả phỏng vấn hay khảo sát để khẳng định tần suất sự cố và độ trễ phát hiện, nên tôi xem đây là các giả định còn cần kiểm chứng, không phải kết quả đã được xác nhận.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

Khó nhất với tôi là xác định đúng bottleneck và diễn đạt vấn đề mà không lẫn giải pháp. “Chưa có AI giám sát camera” không phải một problem đủ tốt; vấn đề cần kiểm chứng là sự cố có bị phát hiện muộn hoặc bỏ sót, gây ảnh hưởng đến an toàn và vệ sinh hay không. Ngoài ra, nhóm chưa có baseline như số vụ mỗi tháng, thời gian từ khi xảy ra sự cố đến khi an ninh biết, hay tỷ lệ trường hợp bị bỏ sót. Khi thiếu dữ liệu, tôi phải phân biệt rõ giữa giả thuyết và sự thật thay vì tự điền số liệu cho đầy đủ biểu mẫu.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

Nếu làm lại, tôi sẽ ưu tiên trao đổi với BQL hoặc nhân viên an ninh ngay từ đầu, xin dữ liệu phản ánh đã ẩn danh và tìm hiểu quy trình phát hiện hiện tại trước khi chọn công nghệ. Tôi cũng muốn kiểm tra sớm xem CCTV có bao phủ đúng khu vực hay không và một ca trực có thể tiếp nhận bao nhiêu cảnh báo. Tôi sẽ phản biện mạnh hơn ở câu hỏi: nếu cảnh báo sai quá nhiều thì giải pháp có thực sự giảm công việc không? Từ đó, nhóm có thể quyết định nên thử nghiệm loại sự cố nào trước và đặt ngưỡng đánh giá rõ ràng.

**6.7. Hiểu bài: giải thích chuỗi problem → quy trình → metric → boundary → mức can thiệp AI → quyết định (5–8 câu).**

Bài toán nhóm lựa chọn là nguy cơ các sự cố thú cưng tại khu vực công cộng bị phát hiện muộn, khiến BQL không thể phản ứng kịp thời. Quy trình hiện tại được giả định là nhân viên nhận phản ánh từ cư dân hoặc theo dõi qua tuần tra và CCTV, rồi mới xác minh và xử lý; các bước này còn cần phỏng vấn để xác nhận. Bottleneck cần kiểm chứng là khoảng thời gian từ lúc sự cố xảy ra đến khi nhân viên nhận biết. Nhóm có thể đánh giá bằng độ trễ phát hiện, tỷ lệ sự cố được cảnh báo đúng, tỷ lệ bỏ sót và số cảnh báo sai trong mỗi ca trực. Boundary của hệ thống là AI không xác định chủ sở hữu, không tự kết luận vi phạm và không tự xử phạt. Mức can thiệp được đề xuất là workflow có Computer Vision phát hiện dấu hiệu nghi vấn, gửi video và thông tin vị trí cho nhân viên an ninh xác minh. Theo đánh giá của tôi, quyết định triển khai thực tế hiện nên là **Not Yet** cho đến khi có bằng chứng về nhu cầu, chất lượng CCTV và hiệu quả cảnh báo trong thử nghiệm nhỏ.

---

## 7. Tài liệu tham khảo

