# Micro-Prototype — Day 18

Lê Quang Huy — 2A202601821. Case B — AI Notes.
Dựng theo [Chặng 2 — Ba Solution Options](../02-three-solution-options.md).

Mở [index.html](index.html) bằng trình duyệt. Một file, không cần cài gì, không gọi mạng.

## Ba option

Trục phân biệt là **ai làm việc biến ghi chú thành thứ dùng lại được**.

| | Option A | Option B | Option C |
|---|---|---|---|
| Phụ trách | **Lê Quang Huy**<br>2A202601821 | Đàm Việt Cường<br>2A202601566 | Trần Đức Bảo<br>2A202601472 |
| Vai trò AI | Không hành động | Ask / Propose | Act |
| AI làm gì | Xếp ghi chú theo slide, tự lưu chống mất file. Không sinh chữ nào. | Soạn sẵn hai nhóm thẻ, mỗi thẻ ghi rõ nguồn slide | Soạn sẵn 100%: 3 ý cốt lõi + 1 mục giải thích + 3 câu tự kiểm tra |
| User làm gì | Kéo mẩu ghi chú vào ba khung mẫu, tự gõ toàn bộ nội dung | Duyệt / sửa / đổi / loại từng thẻ | Đọc luôn, đổi mục tiêu, hoặc rollback |
| Trigger | User chủ động mở khay và kéo thả | Popup đề xuất sau khi học xong | Tự bật khi mở trang ôn bài |
| Đường lùi | Gỡ nguồn, sửa tự do | Hoàn tác từng thẻ | Rollback về ghi chú thô |

**Option A — phần của Huy** — khay ghi chú xếp theo slide bên phải, ba khung mẫu bên trái:
*khung tóm tắt*, *thẻ giải thích*, *thẻ quiz*. Kéo thả được, cũng có nút bấm gắn cho máy
không kéo được. AI chỉ làm hai việc: xếp khay và tự lưu — mốc *tự lưu lúc hh:mm:ss* hiện ở
chân khung là toàn bộ phần AI đóng góp.

**Option B** có hai nhóm thẻ tách riêng — *giải thích* và *tự kiểm tra* — vì hai nguồn
phỏng vấn cho ra hai nhu cầu khác nhau: Hoàn muốn được giải thích, Mai muốn tự kiểm tra.
Tách nhóm để quan sát tester ngả về bên nào.

**Option C** có ô *tùy chỉnh theo mục tiêu* (hiểu sâu / đủ qua bài / ôn nhanh 5 phút). Ô này
đến từ evidence #3: Hoàn cắt bớt việc học theo mục tiêu điểm.

## Những thứ giữ nguyên ở cả ba

Ngữ cảnh, ba mẩu ghi chú fixture, và task của tester — để chênh lệch quan sát được là do
**role split**, không do đổi nội dung.

Task giao cho tester: *"Dùng phương án đang mở để biến các mẩu ghi chú và điểm chưa hiểu
thành một tài liệu hoặc công cụ ôn tập, giúp bạn tự tin trước buổi học tiếp theo."*

Câu này cố ý **không** nói "quiz". Hypothesis đã chốt đặt lõi ở *thứ dùng lại được*; nói
"quiz" là mớm sẵn đáp án, mà chỉ một nguồn (Mai) nhắc tới quiz.

## Nhật ký hành vi

Cột phải ghi tester **đã làm gì**, kèm mốc thời gian và option: kéo mẩu nào vào khung nào,
duyệt hay loại thẻ nào, đổi mục tiêu, bấm rollback. Bấm *Copy nhật ký* để dán vào biên bản.

Nó chỉ ghi thao tác, không ghi ý kiến — để kết luận bám được vào *"Tester đã làm…"* chứ
không trượt sang *"tester nói thích cái này"*.

*Reset về ngữ cảnh ban đầu* xoá sạch state và nhật ký cho tester tiếp theo.

## Dữ liệu trong prototype

Ba mẩu ghi chú và toàn bộ nội dung AI là **content fixture và canned output viết sẵn** —
mục 10 của đề cho phép. Không gọi model thật, không có dữ liệu người dùng thật.

## Còn thiếu

- Chưa chạy buổi test nào với tester thật. Chưa có dòng *"Tester đã làm…"* nào.
- Bảng "Chốt 3 hướng" trong [Solution Parking Lot](../day17-inputs/02-solution-parking-lot.md) vẫn trống.
