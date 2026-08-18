# Chặng 2 — Ba Solution Options (Meaningful Options)

**Nhóm:** cuong  
**Thành viên:** 
1. Lê Quang Huy (2A202601821)
2. Đàm Việt Cường (2A202601566)
3. Trần Đức Bảo (2A202601472)  
**Case B:** AI Notes — Personal Learning Notes  

---

## 1. Mở lại Solution Parking Lot & Kết nối với Evidence Huddle

Từ **Hypothesis Problem đã chốt ở Chặng 1**:
> **Khi** ngồi ôn lại trước buổi học kế tiếp, **người học** khó biến các mẩu ghi chú, ảnh chụp và điểm đánh dấu chưa hiểu thành một thứ dùng lại được **vì** chúng nằm rải rác trên nhiều công cụ và phải tốn công tổng hợp thủ công mới dùng được, **dẫn đến** phải đọc lại tuần tự từ đầu hoặc đẩy sang công cụ ngoài, và không đo được mình đang hổng chỗ nào.

Nhóm 3 thành viên rà soát lại 5 hướng trong Solution Parking Lot từ Day 17 dưới lăng kính của dữ liệu phỏng vấn thực tế từ các nguồn:
- **Nhu cầu của Hoàn (từ phỏng vấn của Huy):** Cần được **giải thích chỗ không hiểu một cách dễ hiểu nhất** theo từng ảnh chụp/slide (khớp Hướng 2).
- **Nhu cầu của Mai (từ phỏng vấn của Cường, Bảo chọn chi tiết #4):** Cần chuyển đổi ghi chú thành **công cụ tự kiểm tra (quiz/đảo kiến thức)** và chống mất file (khớp Hướng 3, 4).
- **Điểm chung của cả nhóm:** Đều nhận thấy người học bị nghẽn ở **chi phí chuyển đổi từ mẩu note thô thành thứ dùng lại được**.

Nhóm phân công 3 thành viên phụ trách thiết kế 3 cơ chế giải pháp với 3 mức độ can thiệp (Role Split) hoàn toàn khác nhau để đưa vào thử nghiệm.

---

## 2. Thiết kế ba Solution Options & Phân công trách nhiệm

### 2.1. Những thành phần BẮT BUỘC GIỮ NGUYÊN (Common Context & Task)

| Thành phần | Quyết định chung cho cả ba Option A / B / C |
|---|---|
| **Target user** | Người học tham gia khóa học AI thực chiến trên nền tảng VLearn. |
| **Situation** | Tối trước buổi học kế tiếp, người học mở lại hệ thống để ôn bài *"Finding & Validating Pain Points"*. Trên bài đã lưu sẵn 3 highlight, 2 note ngắn và 1 ảnh chụp/slide đánh dấu *"Chưa hiểu: Phân biệt Pain vs Consequence"*. |
| **Outcome Task** | *"Trong tình huống này, hãy dùng từng phương án để biến các mẩu ghi chú và điểm chưa hiểu thành một tài liệu/công cụ ôn tập giúp bạn tự tin trước buổi học tiếp theo."* |
| **Desired outcome** | Có tài liệu ôn tập tinh gọn, giải tỏa được điểm chưa hiểu và tự kiểm tra được lỗ hổng kiến thức mà không phải đọc lại toàn bộ bài giảng từ đầu hoặc tốn hàng giờ copy-paste sang nhiều công cụ khác. |
| **Content / Data Fixture** | **3 Snippets dữ liệu thật từ bài 17:**<br>1. *Highlight (Slide 3):* "Problem Hypothesis: Khi [situation], [user] gặp khó khăn [job] vì [barrier], dẫn đến [consequence]."<br>2. *Note ngắn (Slide 7):* "Lưu ý 3 phản xạ: Deflect (Gạt đi), Anchor (Neo lại), Dig (Đào sâu) khi gặp lời khen hoặc đòi hỏi tính năng."<br>3. *Ảnh chụp + Đánh dấu Chưa hiểu (Slide 11):* "Phân biệt Pain (nỗi đau lúc làm job) vs Consequence (hậu quả nếu không giải quyết)." |

---

### 2.2. Bảng so sánh 3 Solution Options (Meaningful Distance)

| Thành phần | Option A (User-Led / Structured Hub) | Option B (Co-Creation / Interactive Co-Pilot) | Option C (AI-Led / Autonomous 1-Click Pack) |
|---|---|---|---|
| **Thành viên phụ trách** | **Lê Quang Huy**<br>2A202601821 | **Đàm Việt Cường**<br>2A202601566 | **Trần Đức Bảo**<br>2A202601472 |
| **Solution Mechanism** | **Interactive Snippet Hub & Manual Binder (Zero-Inference)**: Hệ thống gom tự động các ảnh chụp, highlight và note thành khay Dock bên phải theo slide. Cung cấp sẵn các khung mẫu (Template: Tóm tắt ý chính / Thẻ giải thích / Thẻ Quiz). User tự kéo thả mẩu note vào khung và tự gõ nội dung. | **Interactive AI Co-Pilot (Ask & Propose with Dual Mode)**: AI phân tích các mẩu note/chưa hiểu và đề xuất 2 dạng thẻ: (1) Thẻ tóm tắt & giải thích điểm khó (cho Hoàn) và (2) Thẻ câu hỏi tự kiểm tra kèm trích dẫn slide (cho Mai). User duyệt từng thẻ (*Chấp nhận / Chỉnh sửa / Đổi câu khác*). | **Autonomous Study Digest & Mini-Quiz (Act with Guardrails & Instant Rollback)**: Hệ thống tự động tạo 100% bản tóm tắt trọn gói gồm: 3 ý cốt lõi + 1 mục giải thích điểm khó + Bộ 3 câu trắc nghiệm tự kiểm tra. Cung cấp nút *"Tùy chỉnh theo mục tiêu"* và nút *"Rollback về ghi chú thô"*. |
| **User làm gì?** | Tự kéo thả các mẩu ghi chú vào khung mẫu, tự viết lời giải thích hoặc tự soạn câu hỏi ôn tập theo tư duy cá nhân. | Đọc các thẻ do AI đề xuất, bấm *Chấp nhận*, bấm *Sửa nội dung* hoặc bấm *Đổi câu khác*, quyết định giữ lại những phần mình thực sự cần. | Đọc ngay bản tóm tắt hoặc bấm làm bài trắc nghiệm tự kiểm tra; bấm *Rollback* nếu muốn quay về ghi chú gốc hoặc bấm *Điều chỉnh độ khó*. |
| **AI làm gì?** | **Don't Act / Zero-Inference**: Không tự ý suy luận hay sinh text. Chỉ làm nhiệm vụ sắp xếp, lưu trữ và auto-save đồng bộ dữ liệu chống mất file. | **Ask & Propose**: Đề xuất bản thảo giải thích và câu hỏi dựa trên đúng dữ liệu note của user, hiển thị trích dẫn nguồn slide minh bạch. | **Act with Guardrails**: Tự động biên soạn hoàn chỉnh 100% tài liệu ôn tập và bài trắc nghiệm ngay khi mở trang, hỗ trợ đường khôi phục dữ liệu tức thì. |
| **Trigger** | User chủ động mở khay tổng hợp ghi chú và bắt đầu kéo thả. | Hệ thống hiển thị popup gợi ý: *"AI đã chuẩn bị 1 thẻ giải thích điểm khó và 2 câu hỏi ôn tập từ ghi chú của bạn. Xem ngay?"*. | Tự động kích hoạt khi người học mở trang ôn tập bài cũ. |
| **Trade-off chính** | **Ưu điểm:** Kiểm soát 100%, không lo AI sinh sai lệch.<br>**Nhược điểm:** Tốn nhiều công sức và thời gian tự soạn thảo. | **Ưu điểm:** Cân bằng hoàn hảo giữa tốc độ và quyền kiểm soát; bao phủ cả 2 nhu cầu (giải thích + tự kiểm tra).<br>**Nhược điểm:** Vẫn cần 2-3 lượt click duyệt của học viên. | **Ưu điểm:** Nhanh nhất (0 click ban đầu để có bài ôn tập hoàn chỉnh).<br>**Nhược điểm:** Nếu AI tóm tắt quá sơ sài hoặc sai ý, user có cảm giác bị áp đặt và mất thời gian chỉnh lại. |

---

## 3. Distance Check (Kiểm tra khoảng cách khác biệt)

Hoàn thành ba câu kiểm tra khoảng cách (không nhắc màu sắc, layout hay wording):
- **A khác B vì:** Option A hoàn toàn do con người tự biên tập nội dung từ đầu (AI không suy luận), trong khi Option B AI chủ động đề xuất sẵn các thẻ giải thích và câu hỏi để con người duyệt và tinh chỉnh.
- **B khác C vì:** Option B yêu cầu con người tương tác duyệt từng thẻ (*Ask pattern*), trong khi Option C hệ thống tự động xuất bản trọn gói tài liệu ôn tập ngay lập tức (*Act pattern*) và con người chỉ can thiệp khi muốn rollback/điều chỉnh.
- **A khác C vì:** Option A đòi hỏi 100% nỗ lực biên tập từ con người từ trang giấy trắng, còn Option C là trải nghiệm tự động hóa 1-click toàn diện từ AI.

### Phổ phân chia vai trò (Human–AI Role Spectrum):
```text
[OPTION A - Lê Quang Huy] USER CREATES / INITIATES (Zero-Inference Hub & Manual Binder)
    ↓
[OPTION B - Đàm Việt Cường] USER + AI CO-CREATE (Interactive AI Co-Pilot with Card Review & Dual Mode)
    ↓
[OPTION C - Trần Đức Bảo] AI CREATES / INITIATES, USER REVIEWS (Autonomous Study Digest with Instant Rollback)
```

---

## 4. Đối chiếu Gate 2 (Gate 2 Checklist)

> [!CHECK] **GATE 2 — Meaningful Options**
> - [x] **Cùng chung nền tảng:** Cả ba options đều cùng target user, situation ("trước buổi học kế tiếp"), cùng outcome task, cùng desired outcome và cùng bộ 3 data fixture từ bài 17.
> - [x] **Khác biệt có ý nghĩa về cơ chế:** Phân hóa rõ ràng từ *Zero-Inference* $\rightarrow$ *Ask & Propose (Co-Creation)* $\rightarrow$ *Act with Guardrails (Autonomous)*.
> - [x] **Phân công rõ ràng 3 thành viên:** Mỗi thành viên trong nhóm phụ trách thiết kế và build 1 option độc lập (Huy: Option A, Cường: Option B, Bảo: Option C).
> - [x] **Bao quát cả 2 nguồn evidence:** Option B và C đều thiết kế để đáp ứng đồng thời cả nhu cầu được giải thích điểm chưa hiểu (của Hoàn) và nhu cầu tự kiểm tra kiến thức (của Mai).
> - [x] **Không tạo option bù nhìn:** Cả ba option đều là những hướng giải quyết nghiêm túc, có ưu và nhược điểm thực tế.
