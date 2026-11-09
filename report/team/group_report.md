# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm:
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu):
- Quyết định cuối: Go / Not Yet / No-Go

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |
| 6 | | | | | |
| 7 | | | | | |
| 8 | | | | | |
| 9 | | | | | |
| 10 | | | | | |
| 11 | | | | | |
| 12 | | | | | |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A | | |
| B | | |
| C | | |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: 
├── Opportunity A: 
├── Opportunity B: 
└── Opportunity C: 
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

-

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| | | | | | | | | |
| | | | | | | | | |
| | | | | | | | | |

**Candidate được chọn:**

**Vì sao chọn:**

**Vì sao loại các candidate còn lại:**

**Xử lý bất đồng (nếu có):**

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |
| 6 | | | | | |

*Điền 4–6 giả định; xóa dòng thừa.*

Giả định nhóm kiểm chứng trong buổi này:

### 3.2. Kiểm chứng

Cách đã dùng: Phỏng vấn / Survey / Log, ticket, review

Interview snapshot (mỗi buổi phỏng vấn một bảng, hoặc đặt file trong `report/assets/cp4-interview-snapshot-N.md`):

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | |
| Câu nói đáng nhớ nhất (nguyên văn) | |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | |
| Hiện đang xử lý bằng cách nào (workaround)? | |
| Mất bao lâu, bao lần? | |
| Insight / opportunity rút ra | |

Tổng hợp:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| | | | |

**Nhóm đã sửa problem thế nào sau kiểm chứng:**

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| | | | | | |
| | | | | | |
| | | | | | |

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Sơ đồ (ASCII, Mermaid hoặc link ảnh trong `report/assets/`):

```text

```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |

**Bottleneck chính:**

### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text

```

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | | | |
| Tổng thời gian | | | |
| Số bước thủ công | | | |
| Bottleneck chính | | | |
| Rủi ro mới phát sinh | | | |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | |
| **Quy trình** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** (baseline → target, cách đo) | |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

-

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô:

Vì sao:

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | | | | |
| **Rule** | | | | |
| **Workflow** | | | | |
| **Agent** | | | | |

**Mức chọn:**

**Vì sao không chọn mức đơn giản hơn:**

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | |
| **Judgment** — con người cân nhắc, quyết định gì? | |
| **Action** — hành động cuối cùng là gì, ai làm? | |
| **Outcome** — đo kết quả bằng gì? | |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Bằng chứng:
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào:

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | Ban quản lý, nhân viên an ninh tại các khu chung cư, khu đô thị quy mô lớn. Đối tượng hưởng lợi là cư dân, bao gồm cả người nuôi và không nuôi thú cưng. |
| **Quy trình** | **Hiện tại:** Ban quản lý tiếp nhận phản ánh, kiểm tra camera hoặc cử nhân viên xác minh, xác định sự việc và xử lý theo nội quy. Đây là quy trình giả định, cần xác nhận với ban quản lý thực tế. **Đề xuất:** Camera giám sát → AI phát hiện hành vi nghi vi phạm → ghi nhận hình ảnh, thời gian và vị trí → nhân viên xác minh → xử lý theo quy định. |
| **Bottleneck** | Khó giám sát liên tục nhiều camera và phát hiện kịp thời các hành vi như không dắt dây, không đeo rọ mõm khi bắt buộc, chó cắn người hoặc động vật khác, thú cưng phóng uế không được dọn dẹp. Việc tìm kiếm bằng chứng và xác định chủ nuôi có thể tiêu tốn nhiều nhân lực, đặc biệt tại các khu đô thị lớn. |
| **Impact** | Ảnh hưởng đến an toàn, vệ sinh môi trường, quyền lợi và chất lượng sống của cư dân. Đối với ban quản lý, các sự cố có thể làm tăng khối lượng giám sát, xử lý phản ánh và giải quyết tranh chấp. Hệ thống hướng đến giảm công việc thủ công, nâng cao hiệu quả quản lý và hỗ trợ thực thi nội quy. |
| **Success Metric (baseline → target, cách đo)** | **Baseline:** Chưa có số liệu thực nghiệm về thời gian giám sát, chi phí xử lý hoặc độ chính xác phát hiện. **Target:** Giảm thời gian tìm kiếm và xác minh sự cố; nâng cao tỷ lệ phát hiện đúng; hạn chế cảnh báo sai. **Cách đo:** So sánh quy trình thủ công và quy trình có AI trên cùng tập video; đo Precision, Recall, số cảnh báo sai, thời gian xác minh và khối lượng công việc của nhân viên. Các ngưỡng cụ thể sẽ được xác định trước khi thử nghiệm. |
| **Boundary** | Giai đoạn đầu ưu tiên tận dụng hệ thống CCTV hiện có, chưa bắt buộc triển khai thiết bị IoT. AI chỉ hỗ trợ phát hiện và cung cấp bằng chứng, không tự động kết luận trách nhiệm hoặc xử phạt. Việc xác định chủ nuôi bằng dữ liệu đăng ký và theo dõi liên camera chỉ được triển khai sau khi kiểm chứng độ tin cậy, quyền truy cập dữ liệu và cơ sở pháp lý. |
| **AI intervention point** | Sử dụng Computer Vision để nhận diện thú cưng, dây dắt, rọ mõm và các hành vi liên quan trong video. Hệ thống phân tích chuỗi hình ảnh, đánh dấu sự kiện nghi vi phạm, lưu đoạn video làm bằng chứng và chuyển cảnh báo cho nhân viên kiểm tra. |
| **Mức chọn** | **Workflow:** Kết hợp mô hình Computer Vision, quy tắc xác định hành vi, hệ thống lưu trữ sự cố và bước xác minh của con người. Chưa cần Agent tự chủ trong giai đoạn đầu. |
| **Rủi ro & người kiểm tra** | Rủi ro gồm nhận diện sai, bỏ sót hành vi, chất lượng camera không đủ, nhầm lẫn giữa hành vi bình thường và vi phạm, xác định sai chủ nuôi, lộ dữ liệu cá nhân. Nhân viên an ninh và ban quản lý được phân quyền chịu trách nhiệm xác minh trước khi xử lý. |

### Thay đổi so với v0 và lý do:

*Chưa có nội dung v0 gốc để đối chiếu. Bảng dưới đây nêu các điều chỉnh đề xuất cho v1, không khẳng định đây là những thay đổi đã thực hiện.*

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| Phạm vi dự án | Chưa cung cấp | Chia thành hai giai đoạn: CCTV và thử nghiệm khả thi trước; IoT và vòng đeo thông minh sau. | Giảm chi phí đầu tư ban đầu và kiểm chứng công nghệ trước khi mở rộng. |
| Quy trình | Chưa cung cấp | Bổ sung quy trình từ phát hiện bằng AI đến xác minh và xử lý bởi ban quản lý. | Làm rõ trách nhiệm của hệ thống và con người. |
| Success Metric | Chưa cung cấp | Đo Precision, Recall, cảnh báo sai, thời gian xác minh và khối lượng công việc. | Đánh giá bằng số liệu thay vì chỉ dự đoán lợi ích. |
| Boundary | Chưa cung cấp | Không tự động xử phạt; giới hạn quyền truy cập thông tin cư dân. | Hạn chế rủi ro nhận diện sai và vi phạm quyền riêng tư. |
| AI intervention point | Chưa cung cấp | Tập trung AI vào nhận diện và cảnh báo hành vi nghi vi phạm. | Tránh phụ thuộc ngay từ đầu vào hệ thống theo dõi liên camera và thiết bị IoT. |

### Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | **Độ chính xác cảnh báo (Precision)** | Tỷ lệ cảnh báo đúng đạt ngưỡng được thống nhất trước khi thử nghiệm trên tập video có nhãn độc lập. | Cảnh báo nhầm hành vi bình thường thành vi phạm vượt ngưỡng cho phép. |
| 2 | **Khả năng phát hiện (Recall)** | Phát hiện đủ tỷ lệ các sự cố vi phạm thực tế trong tập video kiểm thử theo ngưỡng đã thống nhất. | Bỏ sót quá nhiều sự cố, đặc biệt các hành vi có nguy cơ ảnh hưởng đến an toàn cư dân. |
| 3 | **Chất lượng bằng chứng** | Mỗi cảnh báo có thời gian, vị trí camera, đoạn video liên quan và mô tả hành vi để nhân viên kiểm tra. | Bằng chứng thiếu, sai thời điểm hoặc không đủ để xác minh sự việc. |
| 4 | **Hiệu quả vận hành** | Thời gian và công sức xác minh mỗi sự cố được xác nhận giảm so với quy trình thủ công, sau khi tính cả thời gian xử lý cảnh báo sai. | Hệ thống làm tăng khối lượng công việc hoặc không tạo ra cải thiện đáng kể. |
| 5 | **An toàn dữ liệu và kiểm soát con người** | Dữ liệu được quản lý theo phân quyền; mọi quyết định xử lý vi phạm đều có người kiểm tra. | Dữ liệu bị truy cập trái phép, xác định sai chủ nuôi hoặc tự động áp dụng hình thức xử phạt khi chưa được xác minh. |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | **TB** | Các vấn đề về an toàn, vệ sinh và quản lý thú cưng có khả năng tạo ra nhu cầu thực tế tại khu dân cư. Nhóm đã thực hiện khảo sát và thu thập đánh giá, nhưng chưa có kết quả chi tiết để xác định mức độ nhu cầu, tần suất vi phạm và khả năng chấp nhận sử dụng của ban quản lý. |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | **TB** | Hệ thống dự kiến cung cấp cảnh báo kèm video bằng chứng để nhân viên xác minh. Tuy nhiên, chưa có sản phẩm mẫu để kiểm tra giao diện, mức độ dễ sử dụng, khả năng sửa kết quả AI hoặc xử lý cảnh báo sai. |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | **Cao** | Công nghệ Computer Vision có thể hỗ trợ nhận diện động vật và vật thể, đồng thời hệ thống CCTV hiện có có khả năng được tận dụng nếu đáp ứng điều kiện kỹ thuật. Tuy nhiên, việc nhận diện bốn nhóm hành vi, thu thập video có nhãn, phát hiện sự kiện theo thời gian và theo dõi thú cưng qua nhiều camera vẫn cần thử nghiệm. |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | **Cao** | Mô hình có tiềm năng giảm chi phí giám sát thủ công và hỗ trợ quản lý khu đô thị lớn. Tuy nhiên, chưa có số liệu chứng minh hiệu quả tài chính. Cần đánh giá chi phí xử lý video, bảo trì, bảo vệ dữ liệu cá nhân, thẩm quyền quản lý và tính hợp pháp của các hình thức xử lý vi phạm. Doanh thu từ tiền phạt chưa thể coi là nguồn thu chắc chắn. |

*Các mức rủi ro trên là đánh giá sơ bộ, chưa phải kết quả kiểm chứng thực nghiệm.*

### 8.2. Kết luận

**Quyết định:** **Not Yet** đối với triển khai thương mại toàn diện; **Go** đối với thử nghiệm khả thi quy mô nhỏ.

**Lý do:**

Dự án hướng đến giải quyết các vấn đề thực tế liên quan đến an toàn, vệ sinh và quản lý thú cưng tại khu dân cư, đặc biệt tại các khu đô thị lớn có nhiều camera giám sát.

Việc ứng dụng Computer Vision để phát hiện hành vi nghi vi phạm là hướng nghiên cứu có cơ sở kỹ thuật. Tuy nhiên, nhóm chưa có sản phẩm mẫu và kết quả thực nghiệm để xác nhận độ chính xác, khả năng triển khai trên hệ thống CCTV hiện có và hiệu quả kinh tế.

Do đó, cần ưu tiên kiểm chứng công nghệ và nhu cầu vận hành trước khi mở rộng sang nhận diện chủ nuôi liên camera hoặc hệ thống vòng đeo IoT.

**Nếu Go — pilot nhỏ nhất:**

1. Lựa chọn một khu vực hoặc một số camera giám sát được cấp phép sử dụng để thử nghiệm.
2. Ưu tiên một đến hai hành vi có thể định nghĩa rõ và có dữ liệu phù hợp, chẳng hạn chó không được dắt dây và hành vi liên quan đến chất thải thú cưng.
3. Thu thập hoặc xây dựng bộ video có nhãn, bao gồm trường hợp vi phạm và không vi phạm.
4. Xây dựng mô hình nhận diện và hệ thống tạo cảnh báo kèm video bằng chứng.
5. Đánh giá Precision, Recall, tỷ lệ cảnh báo sai, thời gian xác minh và chi phí xử lý.
6. Để nhân viên an ninh hoặc ban quản lý xác minh trước khi thực hiện bất kỳ biện pháp xử lý nào.

**Nếu Not Yet — cần kiểm chứng gì trước:**

- Nhu cầu thực tế và khả năng chấp nhận của ban quản lý thông qua khảo sát, phỏng vấn.
- Khả năng thu thập dữ liệu video đủ chất lượng, có nhãn và được phép sử dụng.
- Độ chính xác của từng loại hành vi cần phát hiện.
- Khả năng tích hợp với hệ thống CCTV hiện có.
- Thời gian xử lý, chi phí vận hành và mức tiết kiệm nhân lực thực tế.
- Các yêu cầu pháp lý về dữ liệu cá nhân, camera giám sát, đăng ký thú cưng và thẩm quyền xử lý vi phạm.
- Tính khả thi của theo dõi liên camera và thiết bị IoT trong giai đoạn mở rộng.

**Nếu No-Go — nên làm gì thay AI:**

Ưu tiên cải thiện quy trình đăng ký thú cưng, phổ biến nội quy, tiếp nhận phản ánh từ cư dân, xác minh thủ công qua CCTV và quản lý hồ sơ vi phạm bằng hệ thống phần mềm thông thường.

**Ngưỡng dừng** (nếu sau … mà … thì quay về …):

Trước khi thử nghiệm, nhóm xác định thời gian thử nghiệm, ngân sách tối đa, ngưỡng Precision và Recall tối thiểu, tỷ lệ cảnh báo sai cho phép và yêu cầu bảo vệ dữ liệu.

Nếu sau thời gian thử nghiệm mà mô hình không đạt các ngưỡng đã thống nhất, chi phí vận hành vượt ngân sách hoặc khối lượng xử lý cảnh báo sai làm tăng công việc của nhân viên, nhóm sẽ tạm dừng mở rộng hệ thống và quay lại cải thiện dữ liệu, mô hình hoặc quy trình giám sát thủ công.

Nếu phát sinh vi phạm nghiêm trọng về quyền riêng tư hoặc xử lý vi phạm trái thẩm quyền, phải dừng chức năng liên quan ngay để đánh giá và khắc phục.
---

## 9. Hạn chế và hướng tiếp theo

-

## 10. Tài liệu tham khảo

-
