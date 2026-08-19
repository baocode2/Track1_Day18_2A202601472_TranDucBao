# Chặng 3 — Human–AI Design Pass (Option D)

**Học viên:** Hoàng Minh Quân
**Mã học viên (MHV):** 2A202601574
**Case B:** AI Notes — Personal Learning Notes
**Phương án chịu trách nhiệm thiết kế:** **Option D — On-demand Explain (User chỉ tay, AI giải thích đúng một mẩu)**

Vắng buổi hôm trước. Bắt đầu Day 18 cùng nhóm, nhận một option riêng như Huy (A), Cường (B), Bảo (C).
Cùng ngữ cảnh, cùng 3 snippet, cùng task. Khác ở **role split**.

Đã dựng thật trong [prototype/index.html](prototype/index.html), nút **D — Chỉ đúng chỗ**.

---

## 1. Mục tiêu thiết kế của Option D

Option D đo **baseline đang chạy của Hoàn** (evidence #1): chỗ không hiểu thì gửi đúng chỗ đó cho AI, xin giải thích dễ hiểu. Huddle gọi đây là baseline mọi solution phải vượt. A/B/C đều bỏ qua, nhảy sang làm cả bộ ôn.

D không làm bộ ôn, không làm quiz. AI **im** cho đến khi user chỉ một mẩu. Chỉ sinh **một** lời giải thích, kèm mẩu gốc để đối chiếu.

Câu D trả lời được, A/B/C không trả lời được:

> Pain thật sự là “tốn công làm cả bộ ôn”, hay chỉ là “cần giải thích đúng một chỗ đang vướng”?

---

## 2. Critical moment

User nhìn ba mẩu → **tự chỉ vào một mẩu**, hoặc ngồi chờ máy soạn cả gói.

Đây là chỗ D khác A/B/C: A bắt viết, B đã đưa sẵn bộ thẻ, C đã xong khi mở trang. D không làm gì nếu user không chỉ.

Facilitator ghi: tester chọn Slide 11 (chưa hiểu) trước không, có xin “dễ hơn” không, hay ngồi chờ.

---

## 3. Bốn quyết định thiết kế

### 3.1. Expectation

Trước khi AI viết chữ nào, câu mở đã nói: *"Mình không soạn bộ ôn và không làm quiz. Mình chỉ giải thích đúng một mẩu — và chỉ khi bạn chỉ vào. Mình im cho đến lúc đó."*

Giới hạn: chỉ dựa trên đúng mẩu user chọn, không lấy thêm từ bài khác, không chấm bài, không bao phủ cả buổi học.

### 3.2. Role & Agency

| | Việc |
|---|---|
| **User** | Chỉ một mẩu, đọc lời giải, xin bản dễ hơn, hoặc đóng về ba mẩu thô |
| **AI** | Im. Khi được chỉ: sinh một lời giải thích kèm mẩu gốc và badge nguồn |
| **Pattern** | **Ask on demand** — người gọi, máy trả đúng chỗ. Khác B (máy chủ động đề xuất cả bộ) |

**Khi AI sai:** sai một lời giải. User mất vài giây đọc. Phát hiện được vì mẩu gốc nằm ngay trên lời giải. Đóng một bấm là về ba mẩu thô. Không học nhầm cả bộ như C.

### 3.3. Evidence & Uncertainty

Mỗi lời giải có mẩu gốc + badge *"Dựa vào &lt;slide&gt;"*.

Mẩu Slide 7 quá ngắn: tag đỏ *"AI không chắc — mẩu gốc quá ngắn, nên đối chiếu lại"*. Tín hiệu bám độ dày input, không phải số % bịa.

Xin “dễ hơn” thì thẻ *"bạn xin bản dễ hơn"*.

### 3.4. Control & Recovery

| | Có gì |
|---|---|
| Preview | Không — AI chưa viết gì cho đến khi user chỉ |
| Edit | *Giải thích dễ hơn* — bản thứ hai, cùng một mẩu |
| Reject / Stop | *Đóng, về ba mẩu* — gỡ lời giải, khay ba mẩu hiện lại |
| Undo | Chọn mẩu khác bất cứ lúc nào |

Đường về task ban đầu: một bấm, không hỏi lại.

---

## 4. Human–AI Decision Table (cột D)

| Human–AI decision | Option D (Hoàng Minh Quân) |
|---|---|
| **User làm gì? AI làm gì?** | **User:** chọn đúng một mẩu, đọc, xin dễ hơn, hoặc đóng. **AI:** im cho đến khi được chỉ; rồi giải thích đúng mẩu đó, kèm nguồn. Không quiz, không digest. |
| **AI Act / Ask / Don't Act? Vì sao?** | **Ask on demand.** Đo baseline của Hoàn: giải thích từng chỗ khi user gọi. Không Act vì Act (C) soạn cả gói trước khi user hỏi — đúng rủi ro áp đặt huddle đã ghi. Không Don't Act vì A bắt user tự viết, không phải việc Hoàn đang làm. |
| **User hiểu capability/limit bằng gì?** | Câu mở *trước* khi AI viết: không soạn bộ ôn, không quiz, chỉ một mẩu, im cho đến khi được chỉ. Subtitle khung chat: *"Im cho đến khi bạn chỉ một mẩu · không soạn bộ ôn"*. |
| **Evidence / uncertainty thể hiện thế nào?** | Mẩu gốc nằm trên lời giải; badge nguồn; tag *"AI không chắc"* trên Slide 7; tag *"bạn xin bản dễ hơn"*. |
| **User kiểm soát và recovery thế nào?** | Chọn mẩu khác; *Giải thích dễ hơn*; *Đóng, về ba mẩu* một bấm. |

---

## 5. Distance check

- **D khác A vì:** A bắt user tự viết toàn bộ. D cho AI viết, nhưng chỉ sau khi user chỉ đúng một mẩu.
- **D khác B vì:** B máy đưa sẵn cả bộ thẻ (giải thích + quiz), user chỉ duyệt. D không đề xuất gì, không làm quiz.
- **D khác C vì:** C đã xong 100% khi mở trang. D không làm gì nếu user không chỉ, và không bao giờ làm cả gói.

```text
[OPTION A - Huy] USER CREATES (Don't Act)
    ↓
[OPTION D - Quân] USER POINTS, AI EXPLAINS ONE SNIPPET (Ask on demand)
    ↓
[OPTION B - Cường] AI PROPOSES A SET, USER REVIEWS (Ask / Propose)
    ↓
[OPTION C - Bảo] AI CREATES THE WHOLE PACK (Act)
```

---

## 6. Đối chiếu Gate 3

> [!CHECK] **GATE 3 — Human Control**
> - [x] **Minh bạch phân vai:** AI im cho đến khi được gọi; user quyết chỗ nào cần giải thích.
> - [x] **Agency khớp hậu quả khi sai:** sai một lời giải, mẩu gốc nằm cạnh, đóng một bấm.
> - [x] **Đường kiểm soát & phục hồi:** chọn mẩu khác / xin dễ hơn / đóng về ba mẩu thô.

**Chưa qua được, ghi rõ:**

- D cố ý **không** đáp nhu cầu quiz của Mai. Đó là trade-off, không phải sót: D đo unit of work “một chỗ” của Hoàn. Quiz đã nằm ở B và C.
- Chưa chạy buổi test với tester thật. Chưa có dòng *"Tester đã làm…"*.
