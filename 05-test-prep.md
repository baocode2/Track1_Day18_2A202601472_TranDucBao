# Chặng 5 — Chuẩn bị test

**Nhóm:** cuong
**Thành viên:** Lê Quang Huy (2A202601821), Đàm Việt Cường (2A202601566), Trần Đức Bảo (2A202601472), Hoàng Minh Quân (2A202601574)
**Case B** — AI Notes: Personal Learning Notes

Chạy trên [bản prototype chung](prototype/index.html) — xem [Chặng 4](04-micro-prototype.md).

---

## 1. Relevant context — một câu, tối đa 2 phút

> **"Gần đây bạn có từng ngồi ôn lại một bài học bằng chính ghi chú hoặc ảnh chụp bạn đã lưu
> trong lúc học không?"**

Hỏi trước khi mở prototype. Hỏi **một câu này thôi**, nghe xong thì thôi, không đào tiếp —
Day 18 không phải problem interview.

**Nếu tester trả lời có:** hỏi thêm đúng một câu neo mốc — *"Lần gần nhất là khi nào?"* —
rồi dừng.

**Nếu tester trả lời không:** vẫn chạy test. Vẫn tìm được interaction breakdown: chỗ họ khựng,
chỗ họ bỏ qua evidence, chỗ họ không biết làm gì tiếp. Nhưng **không được rút ra value claim
mạnh** từ người đó — không được viết *"người học thấy phương án này hữu ích"*. Ghi rõ trong
biên bản là tester không có context liên quan.

Câu này bám đúng situation trong Hypothesis Problem đã chốt: *ngồi ôn lại trước buổi học kế tiếp*.

---

## 2. Outcome task — dùng chung cho cả A, B, C và D

> **"Trong tình huống này, hãy dùng từng phương án để biến các mẩu ghi chú và điểm chưa hiểu
> thành một thứ bạn dùng lại được để ôn trước buổi học kế tiếp."**

Đọc nguyên văn câu này, **giữ y hệt ở cả bốn option**. Không đổi chữ giữa chừng.

> **Option D không tạo ra "thứ dùng lại được" nào — và đó là chỗ cần quan sát, không phải lỗi.**
> D chỉ giải thích đúng một mẩu rồi đóng, không để lại artifact. Nếu tester thấy D chưa làm
> xong task, ghi lại đúng câu họ nói. Nếu tester thấy D là đủ, ghi lại luôn — vì lúc đó lõi
> của Hypothesis Problem (*chi phí chuyển note thô thành thứ dùng lại được*) đang bị chính
> tester phản chứng. Facilitator **không được** giải thích hộ, không được nói D làm kiểu khác.

Ba chỗ câu này cố tình tránh:

| Tránh gì | Vì sao |
|---|---|
| Không nói **"quiz"** | Chỉ một nguồn (Mai) nhắc tới quiz; Hoàn không nhắc lần nào. Nói ra là mớm sẵn đáp án cho tester |
| Không nói **nút nào cần bấm** | Task nói kết quả cần đạt. Nói nút là biến test thành hướng dẫn sử dụng |
| Không nói **"tóm tắt"** hay **"sơ đồ"** | Đó là tên các hướng giải pháp. Nói ra là chốt sẵn hình dạng output thay tester |

---

## 3. Observation focus — chọn 5

| # | Thứ cần quan sát | Ghi cụ thể cái gì | Vì sao chọn |
|---|---|---|---|
| 1 | **First action** | Trong 30 giây đầu mỗi option, tester làm gì đầu tiên | Nặng nhất ở **A và D** — hai option duy nhất máy im lúc mở. A: tester tự gõ hay ngồi chờ? D: tester tự chỉ một mẩu hay chờ máy soạn cả gói? Khung chat làm người ta mong máy trả lời. Chờ là dữ liệu, không phải lỗi |
| 2 | **Evidence read / ignored** | Có rê chuột, dừng lại, hay nhắc tới badge *"Dựa vào Slide X"* và tag đỏ *"AI không chắc"* không | Đây là toàn bộ câu hỏi Gate 3. Nếu tester bỏ qua hết tín hiệu nguồn ở Option C thì hàng rào duy nhất của C không hoạt động |
| 3 | **Correction / recovery** | Có bấm *Bỏ thẻ này*, *Hoàn tác*, hay *Bỏ bản này cho mình ghi chú thô* không, và ở thời điểm nào | Đường phục hồi chỉ có giá trị nếu người ta thật sự dùng. Không ai bấm rollback ở C thì cái nút đó là trang trí |
| 4 | **Hesitation** | Chỗ dừng trên 5 giây mà không thao tác gì; ghi lại đang nhìn vào đâu | Chỗ khựng chỉ ra chỗ quyền quyết định không rõ ai cầm |
| 5 | **Option được chọn và trade-off** | Cuối buổi hỏi chọn cái nào trong bốn, và **đổi cái gì lấy cái gì** | Câu tổng hợp bắt buộc. Nếu tester chọn **D**, đó là tín hiệu mạnh nhất buổi test: baseline sẵn có đã đủ, ba option kia đang giải một bài toán chưa chắc tồn tại. Chỉ ghi nhận, không dùng làm bằng chứng solution đúng |

**Hai thứ bỏ, ghi rõ để không ai tưởng là quên:**
- *Misunderstanding* — phần lớn lộ ra qua hesitation và evidence-ignored rồi, giữ thêm là trùng.
- *Help needed* — facilitator không được giải thích (luật 3), nên tín hiệu này bị chặn ngay từ đầu.

---

## 4. Thứ tự chạy — xoay vòng giữa các tester

Không phải tester nào cũng chạy A → B → C → D. Option chạy sau bị option chạy trước làm nhiễu,
và tester mệt dần. Xoay vòng theo hình vuông Latin, mỗi option xuất hiện đúng một lần ở mỗi vị trí:

| Tester | Thứ tự |
|---|---|
| 1 | A → B → C → D |
| 2 | B → D → A → C |
| 3 | C → A → D → B |
| 4 | D → C → B → A |

Bấm **Reset ngữ cảnh** giữa hai tester.

> **Bốn option là dài.** Ước lượng 5–7 phút mỗi option cộng phần hỏi cuối, tức khoảng 25–35
> phút một tester — chưa kể phần xin phép và câu context. Nếu chỉ có 15–20 phút, cắt xuống
> ba option cho tester đó và **ghi rõ bỏ option nào**, thay vì chạy vội cả bốn rồi thu được
> bốn quan sát hời hợt. Bỏ option nào thì theo bảng xoay vòng, bỏ cái đứng cuối.

---

## 5. Luật facilitation

1. **Tester tự điều khiển prototype.** Không cầm chuột hộ, không chỉ tay vào màn hình.
2. **Dùng cùng một task cho A/B/C/D.** Đọc nguyên văn mục 2, không diễn đạt lại.
3. **Không narrate, không giải thích icon.** Tester hỏi cái nút này là gì thì dùng câu cứu hộ số 3.
4. **Không lấp im lặng.** Tester im thì mình cũng im. Đếm thầm tới 5 rồi mới được nói.
5. **Không hỏi "Bạn có thích không?"** Không hỏi ý kiến, không hỏi đánh giá, không hỏi nên có thêm gì.
6. **Tester hỏi nó hoạt động thế nào thì hỏi ngược lại**: *"Theo bạn, nó nên hoạt động như thế nào?"*

**Ba câu cứu hộ — chỉ dùng ba câu này:**
- *"Bạn cứ nói to suy nghĩ của mình nhé."*
- *"Bạn sẽ làm gì tiếp theo?"*
- *"Theo bạn, nó nên hoạt động như thế nào?"*

> Ba lỗi làm hỏng buổi phỏng vấn Day 17 đều là lỗi facilitation, không phải lỗi câu hỏi:
> mớm nguyên nhân trước user, hỏi đuôi *"đúng không?"*, và interviewer nói nhiều hơn người
> được hỏi. Luật 3, 4 và 5 ở trên là để chặn đúng ba lỗi đó.

---

## 6. Biểu mẫu ghi biên bản

Một bảng cho mỗi tester. Chép nhật ký hành vi từ prototype vào cột giữa; cột phải là quan sát
của người ghi, tách riêng.

**Tester:** ……  ·  **Ngày:** ……  ·  **Thứ tự chạy:** ……
**Có context liên quan:** có / không  ·  Nếu có, lần gần nhất: ……

| Observation focus | Tester đã làm gì (thao tác, mốc giờ) | Diễn giải của nhóm |
|---|---|---|
| First action — A | | |
| First action — B | | |
| First action — C | | |
| First action — D | | |
| Evidence read / ignored | | |
| Correction / recovery | | |
| Hesitation | | |
| Option chọn & trade-off | | |

**Câu tester nói, ghi nguyên văn:**
> ……

**Không được viết vào biên bản:** *"tester thích B hơn"*, *"B là phương án đúng"*, *"đã
validated"*. Chỉ ghi thao tác và lời nguyên văn.

---

## 7. Kết luận được phép và không được phép

Cuối buổi, nhóm **được** kết luận theo đúng dạng:

> *"Với Hypothesis Problem này, chúng tôi đã thử bốn cách giải. Tester đã ………, vì vậy
> iteration tiếp theo chúng tôi sẽ ………"*

Nhóm **không được** kết luận *"User đã xác nhận solution này đúng."*

Lý do đứng vững: practice interview Day 17 mới hai nguồn, chưa nguồn nào cho hậu quả định
lượng, và buổi test này đo *interaction*, không đo *value*.

---

## 8. Chuẩn bị trước khi tester ngồi vào

- [ ] Mở [prototype/index.html](prototype/index.html), bấm **Reset ngữ cảnh**
- [ ] **Che banner facilitator** — nó nói thẳng điều đang cần đo
- [ ] Mở sẵn biểu mẫu mục 6
- [ ] Xin phép ghi âm/ghi hình **trước khi** bật máy; không đưa bản ghi lên repo công khai
- [ ] Đọc thuộc ba câu cứu hộ, để không phải nghĩ tại chỗ

---

## 9. Bản chạy tay — cầm theo lúc test

> **Đây không phải buổi phỏng vấn.** Day 17 mới là interview. Hôm nay chủ yếu là **ngồi im và
> nhìn**. Cả buổi facilitator chỉ mở miệng ở bốn thời điểm dưới đây. Ngoài bốn chỗ đó, chỉ
> được dùng ba câu cứu hộ.

### Mốc 1 — Mở đầu (1 phút, trước khi bật máy)

Xin phép ghi âm **trước khi** bật, rồi đọc:

> *"Mình đang thử vài phương án cho một công cụ ghi chú. Mình không kiểm tra bạn — mình kiểm
> tra thiết kế, nên bạn làm gì cũng không sai. Đây là bản dựng thử, bấm hỏng cũng không sao.
> Bạn cứ nói to suy nghĩ của mình nhé."*

Không mô tả trước có mấy phương án, không nói phương án nào có AI.

### Mốc 2 — Câu context (tối đa 2 phút, trước khi mở prototype)

> *"Gần đây bạn có từng ngồi ôn lại một bài học bằng chính ghi chú hoặc ảnh chụp bạn đã lưu
> trong lúc học không?"*

- **Có** → hỏi thêm đúng một câu: *"Lần gần nhất là khi nào?"* → **dừng**, không đào tiếp.
- **Không** → ghi vào biên bản, vẫn chạy test, nhưng **không rút value claim** từ người này.

### Mốc 3 — Mỗi option: đọc task rồi im

Đọc **nguyên văn**, giống hệt cả bốn lần, không diễn đạt lại:

> *"Trong tình huống này, hãy dùng từng phương án để biến các mẩu ghi chú và điểm chưa hiểu
> thành một thứ bạn dùng lại được để ôn trước buổi học kế tiếp."*

Rồi **im**. Trong lúc tester làm, chỉ được dùng ba câu này:

| Khi nào | Nói gì |
|---|---|
| Tester im quá lâu | *"Bạn cứ nói to suy nghĩ của mình nhé."* |
| Tester khựng, không thao tác | *"Bạn sẽ làm gì tiếp theo?"* |
| Tester hỏi nút này là gì / nó chạy thế nào | *"Theo bạn, nó nên hoạt động như thế nào?"* |

Hết một option, hỏi **đúng một câu** rồi chuyển:

> *"Vừa rồi có chỗ nào bạn không chắc chuyện gì đang xảy ra không?"*

Câu này hỏi về **chỗ khó hiểu**, không hỏi thích hay không. Nghe xong ghi lại, không bình luận.

### Mốc 4 — Cuối buổi, sau khi chạy hết (3 câu)

1. *"Trong mấy cái vừa rồi, nếu tối mai bạn phải ôn thật, bạn dùng cái nào?"*
2. *"Chọn cái đó thì bạn mất gì so với mấy cái kia?"*
3. *"Có cái nào bạn chắc chắn không dùng không? Vì sao?"*

Câu 1 hỏi **hành vi sắp tới trong tình huống thật**, không hỏi *"bạn thích cái nào"*. Khác nhau
ở chỗ: thích là ý kiến, dùng là lựa chọn có cái giá đi kèm — và câu 2 chính là để lấy cái giá đó.

### Câu tuyệt đối không hỏi

| Không hỏi | Vì sao |
|---|---|
| *"Bạn có thích không?"* | Lấy ý kiến, không lấy hành vi |
| *"Cái này có hữu ích không?"* | Tester sẽ trả lời lịch sự, không trả lời thật |
| *"Bạn nghĩ nên thêm tính năng gì?"* | Biến tester thành người thiết kế |
| *"Ý bạn là ... đúng không?"* | Nói hộ. Đúng lỗi đã làm hỏng buổi Day 17 |
| *"Chắc là do ... nhỉ?"* | Mớm nguyên nhân trước tester |
| Bất cứ câu nào giải thích icon | Vi phạm luật 3; mất luôn dữ liệu về việc giao diện tự nói được hay không |

### Vừa chạy vừa ghi gì

Prototype tự ghi thao tác ở cột phải. Người ngồi cạnh ghi thêm **năm thứ này**, chỉ ghi cái
quan sát được, không ghi suy đoán:

1. **First action** — 30 giây đầu mỗi option, tester chạm vào cái gì trước.
2. **Evidence** — có dừng lại ở badge *"Dựa vào Slide X"* / tag đỏ *"AI không chắc"* không.
3. **Correction / recovery** — có bấm *Bỏ thẻ*, *Hoàn tác*, *Rollback*, *Đóng* không, lúc nào.
4. **Hesitation** — chỗ dừng trên 5 giây; ghi lại lúc đó đang nhìn vào đâu.
5. **Câu tester tự nói ra** — chép **nguyên văn**, không tóm tắt lại bằng lời mình.

### Kết thúc

- Bấm **Copy nhật ký** dán vào biên bản **trước khi** Reset — reset là mất sạch.
- Bấm **Reset ngữ cảnh** cho tester sau.
- Cảm ơn, không giải thích phương án nào "đúng", không hỏi thêm ý kiến sau khi đã tắt máy.
