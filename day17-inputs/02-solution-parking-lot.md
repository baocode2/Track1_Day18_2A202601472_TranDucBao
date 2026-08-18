# Solution Parking Lot (tách từ Day 17 — CP1)

Nguồn: [01-problem-hypothesis.md](01-problem-hypothesis.md), mục "Solution Parking Lot".

**Problem Hypothesis đang giữ:** Khi ngồi tổng hợp lại kiến thức sau buổi học, HS/SV đọc lại file note nhưng vẫn chưa hiểu vì note chỉ là các mẩu rời chưa được hệ thống thành sơ đồ, dẫn đến học trước quên sau.

Đủ tối thiểu 5 hướng theo yêu cầu Day 18.

| # | Hướng | AI / Không AI | Ghi chú |
|---|---|---|---|
| 1 | Gom highlight cuối bài thành note có cấu trúc (directive gốc) | AI | Hướng gốc của case B |
| 2 | Giải thích ngay tại chỗ khi user đánh dấu "chưa hiểu", không đợi cuối bài | AI | Khác #1 ở thời điểm can thiệp |
| 3 | Tự sinh sơ đồ tư duy nối các khái niệm trong bài với nhau | AI | Đánh thẳng vào "chưa hệ thống thành sơ đồ" |
| 4 | Template ghi chú có sẵn khung (ý chính / thắc mắc / liên hệ) cho user tự điền | Không AI | Baseline không AI |
| 5 | Slide có sẵn mục "tóm tắt + sơ đồ" do giảng viên soạn, học viên chỉ bổ sung | Không AI | Dịch chuyển công việc sang giảng viên |

## Rà soát mechanism / role split (AI hỗ trợ, mục 10 cho phép)

Ba trục để xem hai hướng có thật sự khác nhau hay chỉ khác cách gọi tên.

| # | Can thiệp lúc nào | Ai làm việc hệ thống hóa | Hình dạng output |
|---|---|---|---|
| 1 | Cuối buổi | AI | Note tuyến tính có cấu trúc |
| 2 | Ngay lúc học, theo từng chỗ | AI, user trigger | Lời giải thích rời từng điểm |
| 3 | Sau buổi | AI | Sơ đồ quan hệ giữa khái niệm |
| 4 | Ngay lúc ghi | User | Khung điền sẵn |
| 5 | Trước buổi | Giảng viên | Tóm tắt + sơ đồ soạn sẵn |

Chỗ trùng cần tránh: **1 và 3 gần nhau** — cùng AI làm, cùng sau buổi, chỉ khác hình dạng
output. Lấy cả hai thì mất một slot mà không mua thêm thông tin nào về role split.

Chỗ khó test: **5** đẩy toàn bộ việc sang giảng viên, trong khi tester là HS/SV — khó quan
sát hành vi của chính actor mình đang nghiên cứu.

## Chốt 3 hướng đem đi test ở Day 18

> _Chưa chốt — điền sau khi đọc kỹ đề Day 18._

| Slot | Hướng chọn | Vì sao chọn |
|---|---|---|
| Cách giải 1 | | |
| Cách giải 2 | | |
| Cách giải 3 | | |
