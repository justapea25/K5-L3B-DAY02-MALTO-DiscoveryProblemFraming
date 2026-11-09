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

## 4. Phân tích quy trình hiện tại và đề xuất quy trình có AI

### 4.1. Quy trình hiện tại (As-is)

**Mô tả quy trình:**

1. Ban quản lý (BQL) tiếp nhận phản ánh về sự cố liên quan đến thú cưng.
2. Xác định thời gian và khu vực xảy ra sự cố.
3. Tìm kiếm thủ công trên các camera tại khu vực và khoảng thời gian liên quan.
4. Theo dõi người dắt thú cưng qua nhiều camera để xác định lộ trình di chuyển.
5. Đối chiếu hình ảnh với dữ liệu ra vào, thang máy và thông tin đăng ký thú cưng.
6. Xác định căn hộ liên quan và chuyển thông tin cho BQL xử lý.

**Các điểm nghẽn chính:**

- **Bước 3:** Nhân viên phải tìm kiếm thủ công trên nhiều camera và khung thời gian khác nhau.
- **Bước 4:** Việc theo dõi người và thú cưng qua nhiều camera phụ thuộc vào khả năng quan sát và kinh nghiệm của nhân viên.
- **Bước 5:** Việc đối chiếu hình ảnh với dữ liệu ra vào, thang máy và thông tin đăng ký thú cưng mất thời gian, đặc biệt khi dữ liệu nằm ở nhiều nguồn khác nhau.

Nhìn chung, quy trình hiện tại phụ thuộc nhiều vào thao tác thủ công, khó mở rộng khi số lượng camera và sự cố tăng lên. Thời gian xử lý thực tế chưa được đo lường nên cần khảo sát để xác định đường cơ sở.

### 4.2. Quy trình đề xuất (To-be)

**Mô tả quy trình có AI:**

1. **CON NGƯỜI:** BQL tiếp nhận phản ánh về sự cố.
2. **CON NGƯỜI:** Nhân viên xác định thời gian và khu vực xảy ra sự cố.
3. **RULE:** Lọc camera và khoảng thời gian phù hợp dựa trên vị trí, thời điểm xảy ra sự cố.
4. **AI:** Phân tích video để phát hiện các đối tượng và hành vi bất thường liên quan đến thú cưng.
5. **AI:** Theo dõi người và thú cưng qua các camera liên quan để xác định lộ trình di chuyển.
6. **RULE + AI:** Đối chiếu kết quả phân tích hình ảnh với dữ liệu ra vào, thang máy và thông tin đăng ký thú cưng.
7. **AI:** Tổng hợp và đề xuất Top 3 căn hộ nghi vấn, kèm video, bằng chứng liên quan và điểm tin cậy.
8. **CON NGƯỜI:** Nhân viên BQL kiểm tra bằng chứng, xác minh và chấp nhận hoặc từ chối đề xuất.
9. **CON NGƯỜI:** BQL đưa ra quyết định xử lý sự cố.

**Vai trò và giới hạn của AI:**

- AI hỗ trợ phát hiện đối tượng, theo dõi lộ trình và tổng hợp dữ liệu từ nhiều nguồn.
- AI chỉ đưa ra danh sách căn hộ nghi vấn kèm bằng chứng để hỗ trợ nhân viên kiểm tra.
- Điểm tin cậy chỉ hỗ trợ ưu tiên kiểm tra, không thể hiện xác suất một căn hộ có lỗi hay khẳng định trách nhiệm của cư dân.
- AI không tự kết luận cá nhân hoặc căn hộ vi phạm, không tự động đưa ra quyết định xử lý.
- Nhân viên BQL là người kiểm tra bằng chứng và đưa ra quyết định cuối cùng.

**Cơ chế dự phòng:**

Nếu AI không tìm thấy đối tượng, kết quả có độ tin cậy thấp, dữ liệu không đầy đủ hoặc nhân viên BQL từ chối đề xuất, quy trình sẽ chuyển về phương thức kiểm tra thủ công hiện tại. Các trường hợp bị từ chối cần được ghi nhận để phục vụ đánh giá và cải thiện hệ thống.

### 4.3. So sánh quy trình trước và sau khi ứng dụng AI

| Tiêu chí | Quy trình hiện tại | Quy trình đề xuất |
|---|---|---|
| Số bước | 6 bước | 9 bước |
| Thời gian xử lý | Chưa đo lường | Mục tiêu giảm ít nhất 50% |
| Số bước có thao tác thủ công | 6 bước (bước 1-6) | 4 bước (bước 1, 2, 8, 9) |
| Công việc tốn nhiều thời gian | Tìm kiếm camera, theo dõi đối tượng và đối chiếu dữ liệu thủ công | Kiểm tra, xác minh đề xuất của AI; đây là nút thắt tiềm năng cần đánh giá thực tế |
| Rủi ro | Tốn thời gian, phụ thuộc kinh nghiệm nhân viên, dễ bỏ sót dữ liệu | Theo dõi sai đối tượng, xác định nhầm căn hộ, dữ liệu camera hoặc dữ liệu đối chiếu không đầy đủ |


---

## 5. Problem Statement

### 5.1. Phát biểu vấn đề

| Thành phần | Nội dung |
|---|---|
| **Actor** | Ban quản lý và nhân viên an ninh tại khu dân cư. |
| **Quy trình** | Tiếp nhận phản ánh về sự cố liên quan đến thú cưng, tìm kiếm hình ảnh camera, theo dõi đối tượng và đối chiếu dữ liệu để xác định căn hộ liên quan. |
| **Bottleneck** | Quá trình tìm kiếm thủ công trên nhiều camera, theo dõi người và thú cưng qua nhiều khu vực, đồng thời đối chiếu dữ liệu từ nhiều nguồn khác nhau. |
| **Impact** | Kéo dài thời gian xác minh và xử lý sự cố, tăng khối lượng công việc cho nhân viên, ảnh hưởng đến vệ sinh, an toàn và trải nghiệm cư dân. |
| **Metric** | Mục tiêu giảm ít nhất 50% thời gian xác định căn hộ liên quan so với quy trình hiện tại. Đường cơ sở cần được đo lường trước khi triển khai. |
| **Boundary** | AI chỉ hỗ trợ phân tích hình ảnh, theo dõi đối tượng và đề xuất tối đa 3 căn hộ nghi vấn kèm bằng chứng. AI không tự kết luận vi phạm hoặc quyết định xử lý. Nhân viên BQL phải xác minh trước khi đưa ra quyết định. Nếu kết quả không đáng tin cậy hoặc dữ liệu không đủ, hệ thống chuyển về quy trình thủ công. |

### 5.2. Phản hồi và điều chỉnh Problem Statement

Sau khi trao đổi và nhận góp ý, nhóm nhận thấy một số điểm cần làm rõ:

- **Problem Card đang gộp nhiều loại sự cố:** Các tình huống như thú cưng đi vệ sinh không đúng nơi, thất lạc hoặc gây thương tích có đặc điểm xử lý khác nhau. Nhóm cần xác định rõ phạm vi sự cố ưu tiên.
- **Chưa phân biệt phát hiện đối tượng và phát hiện hành vi:** Nhận diện được chó hoặc người dắt chó chưa đồng nghĩa với việc xác định được hành vi bất thường. Nhóm bổ sung bước phân tích hành vi vào quy trình đề xuất.
- **Chưa có số liệu thời gian xử lý ban đầu:** Nhóm chưa có dữ liệu đo lường thực tế nên chỉ đặt mục tiêu giảm ít nhất 50%, chưa khẳng định đây là hiệu quả đã đạt được.
- **Nguy cơ xác định nhầm căn hộ:** Chỉ dựa vào hình ảnh camera có thể dẫn đến quy kết sai. Nhóm bổ sung bước đối chiếu dữ liệu ra vào, thang máy, thông tin đăng ký thú cưng và yêu cầu nhân viên BQL xác minh trước khi xử lý.

Qua các góp ý, nhóm điều chỉnh quy trình theo hướng AI hỗ trợ phân tích và đề xuất có bằng chứng, trong khi con người vẫn giữ quyền kiểm tra và quyết định cuối cùng.

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
| **Actor** | |
| **Quy trình** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** (baseline → target, cách đo) | |
| **Boundary** | |
| **AI intervention point** | |
| **Mức chọn** | No AI / Rule / Workflow / Agent |
| **Rủi ro & người kiểm tra** | |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| | | | |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | | | |
| 2 | | | |
| 3 | | | |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | | |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | | |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | | |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | | |

### 8.2. Kết luận

**Quyết định:** Go / Not Yet / No-Go

**Lý do:**

**Nếu Go — pilot nhỏ nhất:**

**Nếu Not Yet — cần kiểm chứng gì trước:**

**Nếu No-Go — nên làm gì thay AI:**

**Ngưỡng dừng** (nếu sau … mà … thì quay về …):

---

## 9. Hạn chế và hướng tiếp theo

-

## 10. Tài liệu tham khảo

-
