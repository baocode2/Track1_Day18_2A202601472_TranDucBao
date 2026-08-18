# Micro-Prototype — Day 18

Lê Quang Huy — 2A202601821. Case B — AI Notes.

Mở [index.html](index.html) bằng trình duyệt. Một file, không cần cài gì, không gọi mạng.

## Ba option khác nhau ở đâu

Trục phân biệt là **ai làm việc biến ghi chú thành thứ dùng lại được** — giữ nguyên trục
A/B/C trong [three-option-design-sheet.md](../three-option-design-sheet.md) của Đàm Việt Cường.

| | Option A | Option B | Option C |
|---|---|---|---|
| Vai trò AI | Không hành động | Ask / Propose | Act |
| AI làm gì | Chỉ gom ghi chú và tự lưu. Không sinh nội dung. | Soạn sẵn 3 thẻ, mỗi thẻ ghi rõ nguồn | Sinh trọn bộ 5 thẻ ngay khi kết thúc bài |
| User làm gì | Chọn nguồn, tự gõ câu hỏi và câu trả lời | Duyệt / sửa / đổi câu / loại từng thẻ | Xem, kéo số câu, làm luôn hoặc rollback |
| Đường lùi | Sửa tự do | Hoàn tác từng thẻ | Quay về ghi chú thô |

## Những thứ giữ nguyên ở cả ba

Ngữ cảnh, ba mẩu ghi chú fixture, và task của tester — để chênh lệch quan sát được là do
**role split**, không do đổi nội dung.

Task giao cho tester: *"Từ mấy mẩu ghi chú này, tạo ra một thứ bạn dùng lại được để ôn
trước buổi thực hành kế tiếp."*

Câu này cố ý **không** nói "quiz". Hypothesis đã gộp đặt lõi ở *thứ dùng lại được*; nói
"quiz" là mớm sẵn đáp án cho tester, mà đúng một nguồn (Mai) nhắc tới quiz.

## Nhật ký hành vi

Cột phải ghi lại tester **đã làm gì**, kèm mốc thời gian và option. Bấm *Copy nhật ký* để
dán vào biên bản test. Nó chỉ ghi thao tác, không ghi ý kiến — để phần kết luận bám được
vào *"Tester đã làm…"* chứ không trượt sang *"tester nói thích cái này"*.

*Reset về ngữ cảnh ban đầu* xoá sạch state và nhật ký, chạy lại từ đầu cho tester tiếp theo.

## Dữ liệu trong prototype

Ba mẩu ghi chú và toàn bộ câu hỏi/câu trả lời của AI là **content fixture và canned output
viết sẵn** — mục 10 của đề cho phép. Không gọi model thật, không có dữ liệu người dùng thật.

## Chưa xong

- Ba option chưa được nhóm chốt chính thức; bảng "Chốt 3 hướng" trong
  [Solution Parking Lot](../day17-inputs/02-solution-parking-lot.md) vẫn trống.
- Cường cần xác nhận hypothesis đã gộp, vì design sheet của bạn ấy đang neo output vào "bộ câu hỏi".
