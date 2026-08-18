# Chặng 3 — Human–AI Design Pass (Option B)

**Học viên:** Đàm Việt Cường  
**Mã học viên (MHV):** 2A202601566  
**Case B:** AI Notes — Personal Learning Notes  
**Phương án chịu trách nhiệm thiết kế:** **Option B — Interactive AI Co-Pilot (Dual Mode: Thẻ Giải thích + Thẻ Quiz tự kiểm tra)**  

---

## 1. Mục tiêu Thiết kế của Option B

Option B được tôi thiết kế dựa trên cơ chế **Đồng kiến tạo (Co-Creation)**: AI đóng vai trò người trợ lý soạn thảo (Co-Pilot), tự động phân tích các mẩu ghi chú/ảnh chụp và điểm "Chưa hiểu" của người học để đề xuất nội dung ôn tập; nhưng **người học luôn giữ quyền kiểm soát, chỉnh sửa và quyết định cuối cùng (Human-in-the-loop)**.

---

## 2. Bốn Quyết định Thiết kế Human–AI cho Option B

### 2.1. Quyết định 1: Expectation (Kỳ vọng & Giới hạn năng lực của AI)
- **Trước khi AI hoạt động:** 
  - Giao diện hiển thị thông báo rõ ràng trước khi người học thao tác: *"AI đã quét các ghi chú của bạn và chuẩn bị sẵn 1 thẻ giải thích điểm khó cùng 2 câu hỏi ôn tập để bạn duyệt"*.
  - Người học biết trước dạng nội dung AI sắp đưa ra, không bị bất ngờ hay hiểu lầm.
- **Giới hạn cần nói rõ (Limits):**
  - Banner ghi chú minh bạch: *"Nội dung do AI gợi ý từ slide bài học — Hãy kiểm tra lại trước khi lưu vào bộ ôn thi"*.
  - AI chỉ tóm tắt và đặt câu hỏi dựa trên nội dung bài học có sẵn, không tự ý suy diễn các kiến thức ngoài phạm vi.

### 2.2. Quyết định 2: Role & Agency (Phân vai & Mức độ can thiệp)
- **Tôi làm gì (User Role):**
  - Đóng vai trò là **"Biên tập viên trưởng"**: Đọc lướt các thẻ gợi ý, bấm *[✓ Chấp nhận]* thẻ hay, bấm *[✏️ Sửa]* thẻ chưa chuẩn văn phong, hoặc bấm *[✕ Bỏ qua]* thẻ không cần thiết.
- **AI làm gì (AI Role):**
  - Đóng vai trò là **"Trợ lý soạn thảo" (Drafting Assistant)**: Quét các đoạn text highlight và điểm "Chưa hiểu" để tạo sẵn câu hỏi trắc nghiệm kèm gợi ý đáp án và trích dẫn bài học.
- **Mức độ can thiệp tại Critical Moment:** **ASK & PROPOSE (Đề xuất & Đợi duyệt)**
  - AI không tự ý lưu đè hay xuất bản tài liệu mà bắt buộc phải qua bước người học bấm nút duyệt từng thẻ.
- **Hậu quả khi AI sai:**
  - Nếu AI sinh câu hỏi ngớ ngẩn hoặc sai lệch, người học chỉ tốn **1 click (Bấm "Bỏ qua" hoặc "Đổi câu khác")** mà không bị ảnh hưởng đến dữ liệu gốc. Chi phí sửa sai gần như bằng 0.

### 2.3. Quyết định 3: Evidence & Uncertainty (Minh bạch tín hiệu & Độ tin cậy)
- **Minh bạch nguồn gốc (Evidence Citations):**
  - Trên mỗi thẻ câu hỏi đều có một Badge màu xanh nổi bật: *"🔍 Nguồn: Slide 11 (Điểm đánh dấu Chưa hiểu)"* hoặc *"🔍 Nguồn: Slide 3 (Đoạn text Highlight)"*.
  - Người học luôn biết vì sao câu hỏi này lại xuất hiện và nó bám vào mẩu ghi chú nào.
- **Thể hiện sự không chắc chắn (Uncertainty):**
  - Nếu mẩu ghi chú quá ngắn hoặc tối nghĩa, hệ thống sẽ gắn nhãn cảnh báo: *"⚠️ Độ ưu tiên: Trung bình — Cần người học rà soát kỹ"*.

### 2.4. Quyết định 4: Control & Recovery (Kiểm soát & Phục hồi khi có lỗi)
- **Bộ công cụ kiểm soát trực tiếp trên từng thẻ:**
  1. **Nút `[✏️ Sửa câu hỏi]`:** Cho phép sửa trực tiếp câu hỏi hoặc đáp án theo đúng tư duy cá nhân.
  2. **Nút `[🔄 Đổi câu khác (Regenerate)]`:** Yêu cầu AI sinh lại một câu hỏi khác cùng chủ đề nếu câu hiện tại chưa ưng ý.
  3. **Nút `[✕ Bỏ qua (Reject)]`:** Loại bỏ hoàn toàn thẻ này khỏi bộ ôn tập.
  4. **Nút `[✓ Chấp nhận]`:** Lưu thẻ vào kho Active Recall cá nhân.
- **Đường phục hồi toàn diện (Recovery Path):**
  - Nếu toàn bộ các gợi ý của AI đều không đạt, người học luôn có nút **"⏪ Quay về khay ghi chú thô"** để tự tay sắp xếp/ghi chép mà không bị mất bất kỳ dữ liệu ban đầu nào.

---

## 3. Human–AI Decision Table (Bảng quyết định cá nhân)

| Tiêu chí thiết kế | Thiết kế chi tiết cho Option B (Đàm Việt Cường) |
|---|---|
| **1. User làm gì? AI làm gì?** | **AI:** Quét ghi chú & slide, tạo sẵn thẻ giải thích điểm khó và câu hỏi quiz trắc nghiệm.<br>**User:** Đọc lướt, duyệt từng thẻ, chỉnh sửa văn phong hoặc yêu cầu đổi câu khác. |
| **2. AI Act / Ask / Don't Act? Vì sao?** | **Ask & Propose**: AI đưa ra bản thảo gợi ý và đợi người dùng bấm duyệt, đảm bảo người học luôn nắm quyền kiểm soát tuyệt đối nội dung học tập. |
| **3. User hiểu capability/limit bằng gì?** | Banner thông báo trước khi tạo và dòng nhắc nhở minh bạch: *"Tài liệu gợi ý từ ghi chú cá nhân — Vui lòng kiểm tra trước khi lưu"*. |
| **4. Evidence / Uncertainty thể hiện thế nào?** | Badge trích dẫn chính xác số Slide và loại ghi chú (Highlight / Note / Chưa hiểu); nhãn cảnh báo độ tin cậy. |
| **5. User kiểm soát và Recovery thế nào?** | Hệ thống 4 nút hành động tức thì trên từng thẻ (*Chấp nhận / Sửa / Đổi câu / Bỏ qua*) + Đường phục hồi về ghi chú thô ban đầu. |

---

## 4. Đối chiếu Gate 3 (Human Control Checklist)

> [!CHECK] **GATE 3 — Human Control**
> - [x] **Minh bạch phân vai:** Phân định rõ AI là trợ lý soạn thảo, User là người kiểm duyệt và quyết định.
> - [x] **Mức độ can thiệp an toàn:** Dùng cơ chế *Ask & Propose* với chi phí sửa sai cực thấp (1-click).
> - [x] **Đầy đủ đường kiểm soát & phục hồi:** Có đủ tính năng sửa trực tiếp, đổi câu, bỏ qua và khôi phục ghi chú thô.
