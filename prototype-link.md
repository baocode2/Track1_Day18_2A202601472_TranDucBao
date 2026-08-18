# Prototype Link — Day 18 (Option B: Co-Creation AI Co-Pilot)

**Học viên:** Đàm Việt Cường — **MHV:** 2A202601566  
**Nhóm:** cuong  
**Case B:** AI Notes — Personal Learning Notes  
**Phương án chịu trách nhiệm:** **Option B — Interactive AI Co-Pilot (Dual Mode: Thẻ Giải thích + Thẻ Quiz ôn tập)**  

---

## 1. Đường dẫn trải nghiệm Prototype Option B (Cá nhân)

- **File cục bộ:** [`prototype-option-b.html`](prototype-option-b.html)
- **Cách mở trực tiếp:**
  - Nhấp đúp chuột vào file `prototype-option-b.html` để mở trên bất kỳ trình duyệt web nào (Chrome, Edge, Safari...).
  - Hoặc dùng tiện ích *Live Server* trong VS Code / Antigravity IDE.
- **Link Live Demo Online (GitHub Pages):**  
  `https://damcuong8.github.io/Track1_Day18_2A202601566_DamVietCuong/prototype-option-b.html`

---

## 2. Các Tính năng Tương tác Cốt lõi trên UI Option B

1. **Khay Ghi chú Gốc (Capture Dock):** Hiển thị 3 mẩu dữ liệu thật từ bài 17 (Highlight Slide 3, Note ngắn Slide 7, Điểm Chưa hiểu Slide 11). Bấm vào từng mẩu note sẽ tự động cuộn mượt mà sang thẻ AI tương ứng.
2. **Dual-Mode Co-Pilot Stream (2 Loại Thẻ):**
   - **Thẻ 1 — Giải thích Điểm khó (cho Hoàn):** Tóm tắt điểm mù "Pain vs Consequence" qua ví dụ thực tế; có nút *[✏️ Sửa giải thích]* và *[🔄 Đổi cách giải thích khác]*.
   - **Thẻ 2 & 3 — Câu hỏi Tự kiểm tra Active Recall (cho Mai):** Trắc nghiệm 4 đáp án có badge trích dẫn nguồn (*Slide 3 & 7*); có nút *[✏️ Sửa câu hỏi]*, *[🔄 Đổi câu khác]* và *[✕ Bỏ qua]*.
3. **Bộ công cụ Kiểm soát Human-in-the-loop (Gate 3):**
   - Nút `[⚡ Duyệt nhanh tất cả]` (Batch Review).
   - Nút `[✏️ Sửa]` mở Modal chỉnh sửa văn phong trực tiếp.
   - Nút `[🔄 Đổi câu khác]` sinh ngay phương án thay thế có chiều sâu.
4. **Practice & Review Mode:** Sau khi duyệt xong, bấm `[🚀 Bắt đầu Luyện tập]` để bước vào màn hình trắc nghiệm tương tác thực tế với phản hồi đúng/sai tức thì.
