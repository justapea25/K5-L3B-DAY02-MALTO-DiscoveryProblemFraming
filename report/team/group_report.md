# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: MALTO
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): Hệ thống phát hiện sự cố thú cưng trong khu chung cư
- Quyết định cuối: Go

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

**Bài của nhóm nằm ở ô:** Độ mơ hồ thấp × Độ phức tạp cao → Workflow nhiều bước rõ ràng, chưa chắc cần Agent.

**Vì sao:**

* **Độ mơ hồ thấp:** đầu ra có đúng/sai rõ ràng. Một đoạn video hoặc có thú cưng phóng uế, hoặc không. Con vật trong video hoặc là con đã đăng ký ở căn hộ X, hoặc không phải. Không có nhiều đáp án “chấp nhận được” như khi viết văn bản. Cái khó nằm ở chỗ đầu vào là video không có cấu trúc, chứ không phải ở chỗ đầu ra mơ hồ.
* **Độ phức tạp cao:** bài toán có 3 bước nối tiếp, mỗi bước phụ thuộc bước trước: (1) phát hiện sự kiện → (2) xác nhận thú cưng → (3) truy vết căn hộ. Dữ liệu đến từ ít nhất 3 nguồn: phản ánh của cư dân, video từ nhiều camera (hành lang, thang máy, sảnh), và danh sách thú cưng đã đăng ký.
* Các bước đã biết trước và luôn đi theo một thứ tự cố định, nên viết sẵn được thành Workflow. Không có chỗ nào cần AI tự quyết bước tiếp theo.

### 6.2. So sánh 4 mức

| Mức                             | Phương án cho bài của nhóm                                                                                                                                                                                                                                                                                                                                                                            | Đủ khi nào                                                                                                     | Rủi ro                                                                                                                                                                                                                                  | Chọn?                                                                      |
| -------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| **No AI**(sửa quy trình) | Bắt buộc đăng ký thú cưng; quy định khu vực và thang máy riêng cho thú cưng; cư dân phản ánh kèm giờ và vị trí cụ thể; nhân viên bảo vệ tua camera theo khung giờ được báo                                                                                                                                                                                               | Khi phản ánh có giờ chính xác (sai lệch dưới khoảng 15'), lúc đó tua thủ công chỉ mất vài phút | Thực tế sự cố thường bị phát hiện sau nhiều giờ (vd: sáng hôm sau), khung giờ rộng nên vẫn phải tua 2-3h video; nhân viên ngại làm nên bỏ qua                                                                   | Giữ làm nền (đăng ký thú cưng, mẫu phản ánh), nhưng không đủ |
| **Rule**                   | Dùng motion detection của hệ thống camera để lọc ra các đoạn có chuyển động trong khung giờ và vị trí được báo                                                                                                                                                                                                                                                                        | Khi khu vực đó vắng người, ít chuyển động ngoài thú cưng                                             | Hành lang và sảnh có người qua lại liên tục, nên motion detection bắn ra hàng trăm đoạn và không phân biệt được người, thú cưng hay hành vi phóng uế. Không đạt mức giải được 70–80% trường hợp | Không. Chỉ dùng làm bước lọc thô trước khi đưa vào AI          |
| **Workflow**               | Code lấy video theo vị trí + khung giờ → **AI phát hiện các đoạn có thú cưng dừng lại hoặc có hành vi phóng uế** , trả về mốc thời gian, ảnh và độ tin cậy → ban quản lý xem và xác nhận →**AI gợi ý so khớp với danh sách thú cưng đã đăng ký**→ ban quản lý truy căn hộ qua camera thang máy và hành lang, rồi quyết định xử lý | Khi có camera phủ khu vực chung, video được lưu đủ lâu, và có danh sách thú cưng đăng ký        | AI bỏ sót đoạn video; AI so khớp nhầm con vật; rủi ro quyền riêng tư khi đưa video cư dân vào hệ thống AI                                                                                                              | **Chọn**                                                             |
| **Agent**                  | AI tự nhận phản ánh, tự chọn camera, tự lần theo con vật qua nhiều camera, tự xác định căn hộ và gửi thông báo                                                                                                                                                                                                                                                                          | Khi quy trình không biết trước và cần AI tự khám phá                                                    | AI tự cáo buộc nhầm một căn hộ dẫn đến mâu thuẫn hàng xóm; khó kiểm soát, khó giải thích; chi phí cao. Quy trình vốn đã cố định nên không cần sự linh hoạt này                                         | Không                                                                      |

**Mức chọn:** Workflow. AI chỉ làm 2 bước nhận diện trong video (phát hiện sự kiện, gợi ý so khớp thú cưng). Toàn bộ thứ tự xử lý do code định sẵn, và quyết định cuối cùng thuộc về ban quản lý.

**Vì sao không chọn mức đơn giản hơn:**

* **No AI không đủ** vì bottleneck là thời gian tua video, mà sửa quy trình không làm ngắn được video cần xem khi khung giờ phản ánh rộng nhiều tiếng.
* **Rule không đủ** vì việc phân biệt thú cưng với người và nhận ra hành vi phóng uế là bài toán nhận diện hình ảnh. Không viết được bằng if/else hay ngưỡng chuyển động. Motion detection chỉ giảm được video nhưng vẫn để lại quá nhiều đoạn cần xem.
* Ngược lại, không lên Agent vì các bước đã rõ và cố định. Thêm quyền tự quyết cho AI chỉ làm tăng rủi ro cáo buộc sai mà không thêm giá trị.

### 6.3. AI Canvas rút gọn

| Thành phần                                                                         | Nội dung                                                                                                                                                                                                                                                                                                                                       |
| ------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Prediction**— AI dự đoán / tạo ra gì?                                  | (1) Những đoạn video nào có khả năng chứa sự kiện thú cưng phóng uế (mốc thời gian, camera, ảnh chụp, độ tin cậy). (2) Con vật trong đoạn đó giống con nào trong danh sách thú cưng đã đăng ký (top 3 gợi ý).                                                                                             |
| **Judgment**— con người cân nhắc, quyết định gì?                      | Ban quản lý xem lại đoạn video để xác nhận có đúng sự kiện không, con vật có đúng như AI gợi ý không, bằng chứng đã đủ để liên hệ căn hộ chưa, và xử lý ở mức nào (nhắc nhở, yêu cầu vệ sinh, phạt theo nội quy).                                                                              |
| **Action**— hành động cuối cùng là gì, ai làm?                        | Ban quản lý liên hệ căn hộ liên quan, kèm đoạn video làm bằng chứng, và ghi nhận vào sổ theo dõi. AI không gửi thông báo hay nêu tên căn hộ.                                                                                                                                                                          |
| **Outcome**— đo kết quả bằng gì?                                         | Thời gian tìm ra đoạn video liên quan:  **~2 giờ → ≤10 phút** ; % sự cố truy ra được căn hộ:  **~20% → ≥60%** ; số lần cáo buộc nhầm căn hộ = 0; recall của AI trên bộ video thử:  **≥90%** .                                                                                                   |
| **Input**— AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | Vị trí và khung giờ từ phản ánh (có, cần chuẩn hóa mẫu phản ánh); video từ các camera khu vực đó (có sẵn, nhưng chỉ lưu khoảng 7 ngày, cần quyền truy cập); sơ đồ camera; danh sách và ảnh thú cưng đã đăng ký ( **chưa chắc có sẵn** , cần ban quản lý triển khai đăng ký trước). |
| **Feedback**— lấy phản hồi ở đâu để cải thiện?                      | Mỗi đoạn AI đánh dấu, ban quản lý gắn nhãn đúng/sai. Các sự cố AI bỏ sót nhưng nhân viên tìm thấy thủ công được thêm vào bộ dữ liệu kiểm tra. Kết quả gợi ý thú cưng được đối chiếu với kết quả xác minh cuối cùng. Xem lại hằng tháng để chỉnh ngưỡng.                              |

### 6.4. Hai câu hỏi của Google PAIR

* **Người dùng muốn được hỗ trợ (augment) hay giao hẳn việc (automate)?**

  **Augment.** Ban quản lý muốn bỏ được việc tua video nhàm chán, nhưng việc xác định căn hộ nào vi phạm là chuyện nhạy cảm giữa hàng xóm với nhau. Họ cần tự xem bằng chứng và tự chịu trách nhiệm trước cư dân, nên không muốn một hệ thống tự kết luận.
* **AI sai kiểu nào tệ hơn, báo nhầm hay bỏ sót? Vì sao, và thiết kế đã xử lý thế nào?**

  Câu trả lời khác nhau ở từng bước:

  * **Ở bước tìm đoạn video, bỏ sót tệ hơn.** Báo nhầm chỉ khiến ban quản lý mất thêm vài giây xem một đoạn thừa. Còn bỏ sót thì hệ thống mất tác dụng, vì họ lại phải tua thủ công. Thiết kế: đặt ngưỡng ưu tiên recall (chấp nhận nhiều đoạn nghi vấn hơn), sắp xếp theo độ tin cậy, và luôn có lựa chọn quay về tua thủ công nếu không thấy đoạn đúng.
  * **Ở bước truy ra căn hộ, báo nhầm tệ hơn nhiều.** Cáo buộc sai một hộ gia đình sẽ gây mâu thuẫn, mất niềm tin vào ban quản lý và có thể thành khiếu nại. Thiết kế: AI chỉ đưa ra gợi ý so khớp (top 3, kèm độ tin cậy), không bao giờ nêu tên căn hộ; bắt buộc ban quản lý xem trực tiếp đoạn video trước khi liên hệ; bằng chứng gửi cho cư dân là video gốc chứ không phải kết luận của AI.

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

#### 9.1. Hạn chế

**Về bằng chứng và kiểm chứng**

* Kết quả kiểm chứng chủ yếu dựa trên research thứ cấp, chưa quan sát trực tiếp ban quản lý xử lý một sự cố thật từ đầu đến cuối. Các con số baseline (thời gian tua video, tần suất sự cố) vẫn là ước lượng.

**Về dữ liệu đầu vào**

* Giải pháp phụ thuộc vào hạ tầng camera: góc khuất, camera độ phân giải thấp, ánh sáng ban đêm kém hoặc camera hỏng đều làm AI bỏ sót sự kiện..
* Bước gợi ý so khớp thú cưng cần danh sách và ảnh thú cưng đã đăng ký. Nhiều chung cư hiện chưa có danh sách này, hoặc có nhưng không đầy đủ.
* Nhiều con vật cùng giống, cùng màu lông rất khó phân biệt qua camera. Ở trường hợp này AI chỉ thu hẹp được phạm vi chứ không xác định được chính xác.

**Về quyền riêng tư và pháp lý**

* Đưa video có hình ảnh cư dân vào hệ thống AI đặt ra câu hỏi về sự đồng ý của cư dân, ai được xem video, dữ liệu được lưu ở đâu và trong bao lâu. Nhóm chưa có phương án cụ thể, chưa đối chiếu với quy định bảo vệ dữ liệu cá nhân hiện hành.
* Nếu dùng dịch vụ AI bên ngoài để xử lý video, dữ liệu có thể bị đưa ra khỏi hệ thống của chung cư.

**Về phạm vi giải pháp**

* Hệ thống chỉ giúp tìm bằng chứng sau khi sự cố xảy ra, không ngăn được sự cố. Nguyên nhân gốc (ý thức chủ nuôi, thiếu khu vực cho thú cưng) vẫn cần giải bằng nội quy và quy trình.
* Chưa có bản thử nghiệm trên video thật, nên độ chính xác của AI (recall, tỉ lệ báo nhầm) vẫn là giả định.

#### 9.2. Hướng tiếp theo

1. **Kiểm chứng sâu hơn:** phỏng vấn trực tiếp ban quản lý của 2-3 chung cư; theo dõi 1–2 sự cố thật để đo đúng thời gian tua video và số sự cố bị bỏ qua vì không truy được.
2. **Làm thử nghiệm nhỏ (pilot):** lấy 20-30 đoạn video có sẵn (đã được ban quản lý đồng ý), gắn nhãn thủ công, rồi chạy thử mô hình nhận diện để đo recall và tỉ lệ báo nhầm trước khi làm sản phẩm.
3. **Làm rõ quyền riêng tư:** xây quy định truy cập video (chỉ ban quản lý được xem, có ghi log), ưu tiên xử lý video ngay trên hệ thống của chung cư thay vì gửi ra ngoài, thông báo công khai cho cư dân trước khi áp dụng.

## 10. Tài liệu tham khảo

Anthropic — [Building effective agents](https://www.anthropic.com/research/building-effective-agents): phân biệt Workflow và Agent, nguyên tắc chọn mức đơn giản nhất đủ dùng.

Google PAIR — [People + AI Guidebook: User Needs](https://pair.withgoogle.com/chapter/user-needs/): augment hay automate, báo nhầm hay bỏ sót.

Agrawal, Gans, Goldfarb — [A Simple Tool to Start Making Decisions with the Help of AI (HBR)](https://hbr.org/2018/04/a-simple-tool-to-start-making-decisions-with-the-help-of-ai): AI Canvas.

Microsoft Research — [Guidelines for Human-AI Interaction](https://www.microsoft.com/en-us/research/publication/guidelines-for-human-ai-interaction/): boundary, dễ sửa khi AI sai.
