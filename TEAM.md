# Team

> Điền file này trên repo chung do nhóm trưởng fork. Nhóm điền phần **Thông tin nhóm** và **Thành viên**. Mỗi người tự điền phần của mình trong **Cá nhân**. Không copy file này sang repo khác.

## Thông tin nhóm

- Tên nhóm: MALTO
- Candidate problem nhóm chọn (1 câu): Hệ thống phát hiện sự cố thú cưng trong khu chung cư
- Quyết định cuối (Go / Not Yet / No-Go): Go

## Thành viên

| STT | Họ và tên      | MSSV        | Vai trò trong nhóm             | Tài khoản GitHub |
| --: | ----------------- | ----------- | -------------------------------- | ------------------ |
|   1 | Đậu Hoàng Minh | 2A202604011 | Nhóm Trưởng, Thiết Kế Slide | justapea25         |
|   2 |                   |             |                                  |                    |
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

### HoVaTen-MSSV

**Phần việc phụ trách:**

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

**Điều mình học được từ phần nhóm:**

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
- File cp5-workflow-future.png trong `report/assets/`
- Commit thêm mục 6, mục 9 vào file group report

**Điều mình học được từ phần nhóm:**

Mình học được rằng chọn mức AI phải đi từ mức đơn giản nhất và chỉ áp dụng khi cần thiết. Lúc đầu cả nhóm có suy nghĩ AI làm hết cho cả quy trình nhận diện thú cưng vi phạm, nhưng khi vẽ lại quy trình thì thấy chỉ cần AI ở đúng bước tìm video, còn quyết định căn hộ nào vi phạm phải để con người làm. Mình cũng học được là cùng một lỗi của AI có thể rẻ ở bước này nhưng rất đắt ở bước khác: bỏ sót đoạn video thì chỉ tốn công, nhưng nêu nhầm căn hộ thì gây mâu thuẫn. Cuối cùng, việc card của mình bị loại vì đã có nhiều tool giải quyết giúp mình hiểu một problem tốt không chỉ cần pain thật mà còn phải có khoảng trống thật.
