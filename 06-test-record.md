# Chặng 6 — Biên bản test

**Nhóm:** cuong
**Người ghi:** Lê Quang Huy (2A202601821)
**Case B** — AI Notes: Personal Learning Notes

Chạy trên [prototype chung bốn option](prototype/index.html), theo
[Chặng 5 — Chuẩn bị test](05-test-prep.md).

---

## 1. Cảnh báo về chất lượng dữ liệu — đọc trước khi dùng file này

Dữ liệu hiện có là **báo cáo lại của người ghi**, không phải bản chép nguyên văn tester và
không kèm nhật ký hành vi. Ba hệ quả phải nhớ:

1. **Gần như toàn bộ là ý kiến, không phải hành vi.** Câu *"họ prefer hơn"* là phát biểu sở
   thích. Theo đúng giới hạn của đề, nó **không** đỡ được bất kỳ value claim nào.
2. **Tester đang thiết kế giải pháp hộ nhóm.** Đoạn mô tả cơ chế *"AI phải tự define chỗ chưa
   logic..."* là đề xuất tính năng. Nó đáng ghi lại, nhưng là **tín hiệu về chỗ đang thiếu**,
   không phải bản đặc tả để đi làm.
3. **Chưa có mốc hành vi nào.** Không có first action, không có chỗ khựng, không biết tester
   có đọc badge nguồn không, không biết có bấm rollback không. Năm observation focus ở
   [Chặng 5](05-test-prep.md) mục 3 hiện **trống bốn trên năm**.

Phần dưới tách rõ ba cột: tester nói gì, nhóm diễn giải gì, và chỗ nào chưa có dữ liệu.

---

## 2. Thông tin buổi test

| Mục | Nội dung |
|---|---|
| Tester | ……  *(chưa ghi)* |
| Ngày | ……  *(chưa ghi)* |
| Có context liên quan | ……  *(chưa hỏi hoặc chưa ghi)* |
| Thứ tự chạy | ……  *(chưa ghi)* |
| Nhật ký hành vi | **Chưa có.** Chưa copy trước khi reset, hoặc chưa dán vào đây |

---

## 3. Tester nói gì

> Ghi theo lời người ghi thuật lại. **Chưa phải nguyên văn tester** — chỗ nào nhớ được nguyên
> văn thì bổ sung sau và đánh dấu rõ.

| # | Tester nói / đề xuất | Về option nào | Dạng gì |
|---|---|---|---|
| T1 | Nếu làm theo B thì giảm giao diện xuống còn **hai nút**: *giữ thẻ* hoặc *sửa thẻ* | B | Đề xuất thay đổi giao diện |
| T2 | Thích hơn một phương án **gộp C với D** | C, D | Phát biểu sở thích |
| T3 | Cơ chế mong muốn: sau khi AI tổng hợp, **AI tự xác định chỗ nào chưa logic hoặc thiếu thông tin**, **hỏi lại người dùng**, rồi **liệt kê thành từng mục**; người dùng bấm vào một mục thì AI **giải thích tường minh** phần đó | C + D | Đề xuất cơ chế |

---

## 4. Nhóm diễn giải gì

> Cột này là suy luận của nhóm, **không phải lời tester**.

**Từ T1 — hai nút thay vì bốn.** Option B hiện có bốn nút: *Giữ / Sửa / Đổi thẻ khác / Bỏ*.
Tester nói hai là đủ. Nếu đúng, nghĩa là *Đổi thẻ khác* và *Bỏ* không được dùng tới.

> **Kiểm được bằng dữ liệu, chưa kiểm.** Prototype có ghi lại mọi lần bấm. Mở nhật ký ra xem
> tester có thật sự bấm *Đổi* hoặc *Bỏ* lần nào không. **Nếu không bấm lần nào** thì T1 là
> hành vi có thật, dùng được. **Nếu có bấm mà vẫn nói bỏ đi** thì T1 chỉ là ý kiến, và cái
> đáng tin hơn là thao tác. Đây là chỗ duy nhất trong buổi này còn cơ hội đổi từ ý kiến sang
> hành vi — làm ngay trước khi nhật ký bị reset mất.

**Từ T2 — thích bản gộp C+D.** Chỉ là sở thích, một người. Không kết luận được gì về value.
Nhưng đáng chú ý ở chỗ **không ai chọn A hay B** trong câu trả lời này.

**Từ T3 — chỗ này có tín hiệu thật.** Bóc ra thì đề xuất của tester gồm ba mảnh:

| Mảnh | Đã có ở đâu chưa | Nhận xét |
|---|---|---|
| AI tổng hợp trước, cả gói | **Có** — chính là Option C | Không mới |
| Bấm vào một mục thì được giải thích riêng mục đó | **Có** — chính là Option D | Không mới |
| **AI tự khai báo chỗ nó chưa chắc, rồi hỏi ngược lại người dùng** | **Chưa có ở option nào** | **Đây mới là phần mới** |

Mảnh thứ ba đánh trúng đúng điểm yếu nhóm đã tự ghi ở [Chặng 3](03-human-ai-design-pass.md)
mục 2.2: ở Option C, *AI làm nhiều nhất trong khi sai lại khó phát hiện nhất*, vì người học
chưa nắm bài thì không có cơ sở nào để biết bản tóm tắt sai.

Hiện prototype mới có tín hiệu **bị động**: tag đỏ *"AI không chắc — mẩu gốc quá ngắn"*.
Tester đang đòi tín hiệu **chủ động**: AI nói ra chỗ nó thiếu và hỏi lại. Đó là bước leo thang
thật của cùng một quyết định thiết kế, không phải một tính năng rời.

---

## 5. Nếu nhóm dựng phương án gộp — rủi ro phải xử lý trước

> Chưa dựng. Ghi ra đây để nếu iteration sau làm thì không bỏ sót.

**Rủi ro chính: AI không biết cái nó không biết.** Nếu AI chỉ đánh dấu được những chỗ nó tự
nhận ra là thiếu, thì mọi chỗ **không** bị đánh dấu sẽ mặc nhiên được người học tin là đúng.
Tức là tín hiệu này có thể làm chỗ sai nguy hiểm nhất — chỗ AI sai mà không biết mình sai —
trở nên **khó phát hiện hơn** trước, chứ không dễ hơn.

Cần thử: giới hạn phần AI tự đánh dấu vào thứ kiểm được một cách máy móc — ví dụ *"mẩu ghi
chú gốc chỉ có một dòng"*, *"mục này không có mẩu nào đỡ"* — thay vì để AI tự đánh giá
*"chỗ này chưa logic"*.

**Rủi ro thứ hai: hỏi ngược lại là thêm việc.** Chính pattern Act ở Option C được chọn để bỏ
hết thao tác. Chèn một vòng hỏi đáp vào giữa là kéo nó về gần Option B. Phải đo xem người
học chịu trả lời mấy câu trước khi bỏ ngang.

---

## 6. Kết luận

> **Với Hypothesis Problem này, chúng tôi đã thử bốn cách giải. Tester đã đề xuất rút Option B
> xuống hai thao tác giữ/sửa, và nói muốn một phương án gộp Option C với Option D trong đó AI
> tự nêu chỗ nó còn thiếu rồi hỏi lại. Vì vậy iteration tiếp theo chúng tôi sẽ đối chiếu đề
> xuất đó với nhật ký hành vi để biết nút nào thật sự không được dùng, và dựng thử một tín
> hiệu "AI tự khai báo chỗ chưa chắc" giới hạn trong những thứ kiểm được máy móc.**

Nhóm **không** kết luận *"User đã xác nhận solution này đúng."*

Lý do: một tester, dữ liệu thu được gần như toàn bộ là sở thích và đề xuất tính năng, chưa có
mốc hành vi nào, và chưa nguồn nào cho hậu quả định lượng.

---

## 7. Còn thiếu — làm trước khi nộp

- [ ] **Dán nhật ký hành vi vào mục 2.** Việc gấp nhất: reset là mất.
- [ ] Đối chiếu T1 với nhật ký — tester có bấm *Đổi thẻ khác* hoặc *Bỏ* lần nào không.
- [ ] Điền tên tester, ngày, thứ tự chạy, và có context liên quan hay không.
- [ ] Bổ sung **first action** của từng option — nhất là A và D, hai option máy im lúc mở.
- [ ] Tester có đọc badge nguồn và tag *"AI không chắc"* không.
- [ ] Ở C có bấm rollback không; ở D có xin *"giải thích dễ hơn"* không.
- [ ] Chép nguyên văn ít nhất một câu tester tự nói ra.
