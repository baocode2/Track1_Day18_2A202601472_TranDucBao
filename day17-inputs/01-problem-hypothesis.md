# CP1 — Problem Hypothesis

Case B — AI Notes. Làm một mình.

## 1. Solution

Directive: AI Notes tạo bản ghi chú, chỉnh sửa xác nhận trước khi lưu.

Chỗ mô tả giao diện/tên feature: "AI Notes", nút highlight, đánh dấu "Chưa hiểu", màn hình cuối bài.

Bỏ hết đi thì khả năng cần tạo ra: tổng hợp những highlight người dùng đánh dấu là chưa hiểu.

Không phải cách duy nhất — có thể giải thích luôn tại thời điểm đánh dấu (kèm confirmation) thay vì gom lại cuối bài.

Capability trung tính: biến những gì người học đánh dấu trong lúc học thành một bản tổng hợp có hệ thống để dùng lại về sau.

## 2. Change

Solution → user highlight + confirm chỗ chưa hiểu → note được hệ thống hóa thành sơ đồ → user tổng hợp lại được kiến thức, đỡ học trước quên sau

Các thay đổi kỳ vọng:
- User phải confirm sau khi highlight thì AI mới ghim thẻ giải thích vào.
- User phải hình thành thói quen highlight chỗ chưa hiểu.
- User phải giao tiếp với agent để ra được thẻ tổng hợp kiến thức cho mỗi vùng highlight.

Output (mình tạo ra được): file note tổng hợp, hệ thống hóa thành sơ đồ tư duy.
Outcome (chỉ ảnh hưởng, không kiểm soát được): user thật sự mở lại note và nhớ được bài.

## 3. Actor

> _Toàn bộ bảng này là giả định, chưa kiểm chứng._

| Actor | Đang làm gì | Pain / hậu quả | Hưởng lợi gì |
|---|---|---|---|
| Học sinh, sinh viên | Nghe giảng, highlight và note lại chỗ chưa hiểu, sau buổi ngồi ôn lại. Phải đổi hành vi thì outcome mới xảy ra | Trải nghiệm pain trực tiếp: đọc lại note mà vẫn không nối được thành hệ thống, học trước quên sau | Tổng hợp được kiến thức, ôn nhanh hơn, đỡ quên |
| Giảng viên | Soạn bài, giảng, trả lời thắc mắc trên lớp và sau buổi | Phải giảng lại kiến thức cũ, lớp đi chậm, không biết ai đang hổng chỗ nào | Học viên vào lớp đã nắm bài, đỡ phải nhắc lại, dạy được sâu hơn |
| SV cùng coach lab | Học và làm lab cùng nhóm, hỏi bài lẫn nhau | Phải giải thích lại phần bạn cùng nhóm chưa nắm, nhóm bị chậm | Cả nhóm cùng nhịp, lab chạy nhanh hơn |
| Nhà trường | Vận hành chương trình, theo dõi kết quả học | Kết quả học tập và tỉ lệ hoàn thành môn thấp | Hưởng lợi gián tiếp: chất lượng đầu ra và mức độ hài lòng của người học |

Chọn actor: học sinh, sinh viên.
Vì sao: nhóm này được include vào khá nhiều phần và là nhóm chịu ảnh hưởng chính.

## 4. Situation & Job

Situation chốt: **khi đang ngồi tổng hợp lại kiến thức sau buổi học** (không phải lúc đang nghe giảng).

Khi ngồi tổng hợp lại kiến thức, HS/SV đang cố hiểu và hệ thống lại ý chính của bài bằng cách đọc lại phần đã highlight và note trong lúc học.

JTBD: Khi ngồi tổng hợp lại kiến thức sau buổi học, tôi muốn hệ thống nhanh các ý chính và những chỗ tôi đánh dấu chưa hiểu, để có thể nhớ được bài và chuẩn bị cho bài sau.

## 5. Pain

Pain A — Khi ngồi tổng hợp kiến thức, HS/SV đọc lại file note nhưng vẫn chưa hiểu vì note chỉ là các mẩu rời chưa được hệ thống thành sơ đồ, dẫn đến học trước quên sau.

Pain B (cạnh tranh) — Khi ngồi tổng hợp kiến thức, HS/SV không tổng hợp được vì nhìn lượng kiến thức lớn thấy ngợp nên mất tập trung và nản, dẫn đến bỏ dở việc ôn.

Khác nhau ở đâu: A là vấn đề **cấu trúc thông tin** (có đọc, nhưng không nối được thành hệ thống). B là vấn đề **động lực/chú ý** (không đọc tới nơi vì nản). Hai cái không thể cùng là nguyên nhân chính.

Chọn: A
Lý do: A nghe khả thi hơn.

## 6. Evidence

> _AI draft — cần rà lại._

| Cần kiểm tra | Tin hơn nếu | Nghi ngờ / bác bỏ nếu |
|---|---|---|
| Situation có thật | Kể được lần gần nhất ngồi ôn lại và có mở note cũ ra | Không nhớ nổi lần gần nhất nào mở lại note |
| Pain có ý nghĩa | Đọc note xong vẫn phải đi tìm nguồn khác để hiểu | Đọc note là đủ, không cần làm gì thêm |
| Workaround tồn tại | Đã tự vẽ sơ đồ, chép lại, hỏi bạn, hoặc hỏi AI để nối các mẩu note | Không làm gì thêm ngoài đọc lướt |
| Consequence tồn tại | Nêu được lần cụ thể bị quên/mất thời gian/làm lại | Không nêu được hậu quả nào cụ thể |
| Pattern lặp lại | Chuyện này xảy ra hầu như sau mỗi buổi học | Chỉ xảy ra một lần vì môn đó khó bất thường |

Workaround giả định (chưa kiểm chứng): tự chép lại note ra vở/sơ đồ, hỏi bạn, tra lại slide, hỏi ChatGPT.

## Chốt

Problem Hypothesis: Khi ngồi tổng hợp lại kiến thức sau buổi học, HS/SV đọc lại file note nhưng vẫn chưa hiểu vì note chỉ là các mẩu rời chưa được hệ thống thành sơ đồ, dẫn đến học trước quên sau.

Phải đúng điều gì thì mới đứng vững:
- Họ thật sự có ghi note/highlight trong lúc học.
- Họ thật sự có mở lại note đó sau buổi học.
- Lúc mở lại, họ vướng ở việc nối các mẩu rời thành hệ thống.

Cái gì làm nó sai:
- Họ không hiểu bài vì mất tập trung và chán nản, chứ không phải vì note thiếu cấu trúc (→ Pain B đúng).
- Họ không bao giờ mở lại note (→ pain nằm ở chỗ khác hẳn).
- Họ đọc note là hiểu, không cần hệ thống hóa gì thêm (→ không có pain).

## Solution Parking Lot

> _AI draft — cần rà lại._

| # | Hướng | AI / Không AI |
|---|---|---|
| 1 | Gom highlight cuối bài thành note có cấu trúc (directive gốc) | AI |
| 2 | Giải thích ngay tại chỗ khi user đánh dấu "chưa hiểu", không đợi cuối bài | AI |
| 3 | Tự sinh sơ đồ tư duy nối các khái niệm trong bài với nhau | AI |
| 4 | Template ghi chú có sẵn khung (ý chính / thắc mắc / liên hệ) cho user tự điền | Không AI |
| 5 | Slide có sẵn mục "tóm tắt + sơ đồ" do giảng viên soạn, học viên chỉ bổ sung | Không AI |
