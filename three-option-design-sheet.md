# Three-Option Design Sheet — Day 18

**Học viên:** Đàm Việt Cường | **MHV:** 2A202601566 | **Nhóm:** cuong  
**Case nghiên cứu:** Case B — AI Notes: Personal Learning Notes  

---

## PHẦN 1: TỔNG HỢP EVIDENCE TỪ DAY 17 (CHẶNG 1)

### 1.1. Bảng đối chiếu Evidence (Evidence Huddle)

| Practice Note / Nguồn | User đã thực sự làm/nói gì? (Observed) | Điều nhóm đang diễn giải (Interpreted) |
|:---:|---|---|
| **Note 1 (Bạn Mai - 01317)** | Xuất slide VLearn sang iPad để viết tay + gõ vội vào Notepad trên máy tính. Lúc ôn tập: *"nếu ghi chú ở iPad... chỉ có cách là đọc lại từ đầu đến cuối thôi... không thể đảo lẫn kiến thức lên để biết mình đang quên hay thiếu chỗ nào"*. | Học viên có nhu cầu chủ động kiểm tra lỗ hổng kiến thức (active recall) bằng quiz/flashcard đảo ngẫu nhiên thay vì chỉ đọc lại thụ động (passive reading). |
| **Note 2 (Bạn Mai - 01317)** | *"Thực ra mình cảm thấy tốn thời gian nhất là mình sẽ lại phải từ cái file ghi chú đấy để tổng hợp ra... mấy cái phần mềm làm quiz để có thể tạo ra được những câu hỏi... Nhưng ghi chú trên giấy tay thì tổng hợp lại khá là khó"*. | Rào cản lớn nhất không phải là ghi chú, mà là chi phí cơ hội và thời gian chuyển đổi các mẩu ghi chú thô/viết tay thành công cụ tự kiểm tra kiến thức. |
| **Note 3 (Bạn Mai - 01317)** | *"Notepad ở máy tính thì bình thường là lưu rất linh tinh nên sẽ bị miss rất nhiều ghi chú quan trọng và đến lúc tìm lại thì-- hoặc là có thể chưa Ctrl S... sẽ bị mất"*. | Học viên gặp rủi ro phân mảnh dữ liệu (fragmentation) và mất mát dữ liệu khi dùng nhiều công cụ rời rạc không đồng bộ tự động. |

### 1.2. Thảo luận nhanh & Pattern nhận diện
- **Situation & Behavior lặp lại:** Học viên luôn thực hiện hành vi ghi chép trong buổi học trực tiếp nhưng dùng công cụ phân tán (iPad + Notepad + Slide).
- **Evidence bất ngờ:** Học viên không chỉ muốn "tóm tắt lại để đọc", mà mục tiêu tối hậu là muốn **tạo câu hỏi quiz/trắc nghiệm tự kiểm tra lỗ hổng kiến thức** nhưng bị chặn lại vì chi phí tổng hợp thủ công quá lớn.
- **Điều vẫn chỉ là suy đoán:** Liệu một bộ câu hỏi ôn tập do AI sinh tự động 100% có thực sự đánh đúng vào điểm học viên chưa hiểu, hay học viên vẫn muốn tự tay chọn lọc và biên tập từng câu hỏi?

### 1.3. Chốt Hypothesis Problem (Gate 1 Passed)

> **Khi** vừa học xong bài học dài và phức tạp trên VLearn, **học viên** gặp khó khăn trong việc **tự tạo bộ tài liệu ôn tập và câu hỏi tự kiểm tra kiến thức cá nhân hóa (Active Recall / Quiz)** **vì** các dấu vết ghi chú, highlight và điểm chưa hiểu nằm phân mảnh rải rác trên nhiều công cụ mà không có cách chuyển đổi nhanh thành dạng câu hỏi ôn tập, **dẫn đến** tốn nhiều giờ đọc lại toàn bộ bài giảng từ đầu một cách thụ động, dễ làm thất lạc kiến thức trọng tâm và không đo lường được mình đang hổng chỗ nào trước buổi thực hành tiếp theo.

- **Evidence ban đầu hỗ trợ giả thuyết:** Lời kể và trích dẫn trực tiếp của học viên Mai (01317) về việc bất tiện khi ôn tập trên iPad, tốn thời gian soạn quiz thủ công và mất note trên Notepad.
- **Điều vẫn chưa được chứng minh:** Mức độ can thiệp của AI đến đâu là tối ưu (User tự kéo thả vs. AI gợi ý từng câu vs. AI tự động tạo sẵn 100% kèm review)?

---

## PHẦN 2: THIẾT KẾ BA SOLUTION OPTIONS (CHẶNG 2)

### 2.1. Những thành phần giữ nguyên chung (A / B / C)
- **Target User:** Học viên tham gia khóa học AI thực chiến trên nền tảng VLearn.
- **Situation:** Học viên vừa kết thúc bài học phức tạp *"Finding and Validating Pain Points"*, trên hệ thống đã lưu 3 đoạn text highlight, 2 mẩu ghi chú ngắn và 1 slide đánh dấu *"Chưa hiểu: Phân biệt Pain vs Consequence"*.
- **Task của Tester:** *"Tạo một bộ câu hỏi ôn tập (Personal Review Quiz) từ các ghi chú của bài học vừa qua để tự kiểm tra kiến thức trước buổi thực hành tiếp theo."*
- **Desired Outcome:** Có ngay một bộ câu hỏi tự kiểm tra kiến thức tinh gọn, đúng trọng tâm phần mình còn hổng, có thể đảo ngẫu nhiên để luyện tập và đảm bảo không bị mất dữ liệu.
- **Content/Data Fixture:**
  - *Snippet 1 (Highlight - Slide 3):* "Problem Hypothesis: Khi [situation], [user] gặp khó khăn [job] vì [barrier], dẫn đến [consequence]."
  - *Snippet 2 (Note ngắn - Slide 7):* "Lưu ý 3 phản xạ: Deflect (Gạt đi), Anchor (Neo lại), Dig (Đào sâu) khi gặp lời khen hoặc đòi hỏi tính năng."
  - *Snippet 3 (Đánh dấu Chưa hiểu - Slide 11):* "Phân biệt Pain (nỗi đau/khó khăn lúc làm job) vs Consequence (hậu quả/chi phí nếu không giải quyết)."

### 2.2. Bảng so sánh 3 Solution Options

| Thành phần | Option A (User-Led / Structured Binder) | Option B (Co-Creation / Interactive AI Co-Pilot) | Option C (AI-Led / Autonomous Smart Pack) |
|---|---|---|---|
| **Solution Mechanism** | **Interactive Snippet Binder & Manual Quiz Creator**: Gom toàn bộ note/highlight vào khay dock bên phải. User tự kéo-thả vào khung câu hỏi, tự chọn dạng quiz (Flashcard / Multiple Choice). | **AI Suggestion & Structuring Co-Pilot**: AI phân tích các mẩu note/chưa hiểu và gợi ý sẵn 3 câu hỏi trắc nghiệm kèm trích dẫn nguồn. User duyệt từng thẻ (*Accept / Edit / Reject*). | **Autonomous Study-Pack Generator**: Hệ thống tự động biên soạn 100% bộ Smart Quiz 5 câu có phân hóa độ khó ngay khi kết thúc bài. User chỉ việc nhấn *"Làm Quiz ngay"* hoặc bấm *"Điều chỉnh / Rollback"*. |
| **User làm gì?** | Tự kéo thả các mẩu ghi chú vào khung câu hỏi, tự gõ phương án trả lời và thiết lập thẻ ôn tập. | Đọc các câu hỏi trắc nghiệm do AI đề xuất, bấm *Chấp nhận*, bấm *Sửa nội dung* hoặc bấm *Đổi câu khác*. | Nhìn tổng thể gói Quiz được tạo sẵn, nhấn bắt đầu ôn tập ngay hoặc kéo thanh trượt điều chỉnh mức độ thử thách. |
| **AI làm gì?** | **Don't Act / Zero-Inference**: Không sinh nội dung, chỉ tự động phân loại nguồn và auto-save chống mất file. | **Ask & Propose**: Đề xuất bản thảo câu hỏi và đáp án dựa trên đúng dữ liệu note của user, trích dẫn rõ slide nguồn. | **Act with Guardrails**: Tự động tạo hoàn chỉnh bộ quiz + tóm tắt bài học, cung cấp nút phục hồi/quay lại dữ liệu thô bất cứ lúc nào. |
| **Trigger** | User chủ động nhấn mở khay "Tạo Quiz từ Ghi chú". | Hệ thống hiển thị popup gợi ý nhẹ nhàng: *"AI đã chuẩn bị 3 câu hỏi ôn tập từ 2 điểm Chưa hiểu của bạn. Xem ngay?"*. | Tự động kích hoạt khi học viên nhấn nút "Hoàn thành bài học". |
| **Trade-off chính** | **Ưu điểm:** Kiểm soát 100%, không lo AI bịa đặt (hallucination).<br>**Nhược điểm:** Tốn công sức và thời gian soạn câu hỏi thủ công. | **Ưu điểm:** Cân bằng hoàn hảo giữa tốc độ và quyền kiểm soát; duyệt nhanh từng câu.<br>**Nhược điểm:** Vẫn cần 2-3 lượt click duyệt của học viên. | **Ưu điểm:** Nhanh nhất (0 click ban đầu để có bài ôn tập ngay).<br>**Nhược điểm:** Nếu AI tạo câu hỏi lệch trọng tâm, user có cảm giác bị áp đặt và mất thời gian chỉnh lại. |

### 2.3. Distance Check (Kiểm tra khoảng cách khác biệt)
- **A khác B vì:** Option A hoàn toàn do con người tự biên soạn nội dung câu hỏi (AI không suy luận), trong khi Option B AI chủ động soạn sẵn câu hỏi mẫu và user giữ quyền duyệt/sửa từng câu.
- **B khác C vì:** Option B yêu cầu user tương tác duyệt từng thẻ câu hỏi (Ask pattern), trong khi Option C hệ thống tự động xuất bản trọn gói bài quiz ngay lập tức (Act pattern) và user chỉ can thiệp khi muốn rollback/điều chỉnh.
- **A khác C vì:** Option A đòi hỏi 100% nỗ lực biên tập từ user từ trang giấy trắng, còn Option C là trải nghiệm 1-click tự động hóa toàn diện từ AI.

---

## PHẦN 3: HUMAN–AI DESIGN PASS (CHẶNG 3)

### 3.1. Bảng quyết định thiết kế Human–AI (Human–AI Decision Table)

| Tiêu chí thiết kế | Option A (User-Led) | Option B (Co-Creation) | Option C (AI-Led) |
|---|---|---|---|
| **1. Role & Agency (User & AI làm gì?)** | User nắm 100% quyền sáng tạo nội dung. AI chỉ làm nhiệm vụ lưu trữ và hiển thị khay ghi chú trực quan. | User đóng vai trò "Biên tập viên / Người kiểm duyệt". AI đóng vai trò "Trợ lý soạn thảo đề xuất". | AI đóng vai trò "Giảng viên tự động soạn đề". User đóng vai trò "Người trải nghiệm & Người quyết định cuối cùng". |
| **2. Decision (Act / Ask / Don't Act? Vì sao?)** | **Don't Act**: AI không suy luận hay tự sinh nội dung vì người dùng muốn tự tay tổng hợp chính xác theo tư duy cá nhân. | **Ask / Propose**: AI đưa ra bản thảo gợi ý kèm nút hành động rõ ràng (*Duyệt / Sửa / Xóa*) để user luôn làm chủ. | **Act with High Transparency**: AI tự động tạo gói quiz ngay lập tức để tiết kiệm tối đa thời gian cho học viên, nhưng đi kèm cơ chế minh bạch nguồn. |
| **3. Expectation & Limit (Hiểu năng lực/giới hạn)** | Giao diện ghi rõ: *"Ghi chú được trích xuất nguyên văn từ bài học và tự động lưu đám mây"*. | Banner ghi rõ: *"Câu hỏi được tạo tự động từ ghi chú của bạn. Hãy kiểm tra nội dung trước khi lưu"*. | Thông báo: *"Đã tạo 5 câu hỏi dựa trên nội dung bài học. Độ chính xác tham chiếu slide đạt 100%"*. |
| **4. Evidence & Uncertainty (Minh bạch tín hiệu)** | Mỗi thẻ ghi chú hiển thị rõ: Tên Slide, Vị trí highlight, Thời gian ghi chép. | Mỗi câu hỏi AI sinh đều có badge đính kèm: *"Dựa vào Highlight Slide 3"* hoặc *"Dựa vào điểm Chưa hiểu Slide 11"*. | Hiển thị trích dẫn nguồn (Source Citation) và tỷ lệ phủ kiến thức của bộ câu hỏi đối với các điểm mấu chốt. |
| **5. Control & Recovery (Kiểm soát & Phục hồi)** | Nút Undo/Redo, kéo thả tự do, chỉnh sửa text trực tiếp bất cứ lúc nào. | Nút *Regenerate* (đổi câu khác), nút *Edit* trực tiếp trên thẻ, nút *Reject* loại bỏ câu không thích. | Nút *Chỉnh sửa bộ đề*, nút *Thêm câu hỏi thủ công*, và nút *Khôi phục về ghi chú gốc* (Instant Reset/Rollback). |

---

## PHẦN 4: THIẾT KẾ MICRO-PROTOTYPE & TEST PROTOCOL

### 4.1. Cấu trúc màn hình Micro-Prototype
Cả 3 Options đều được tích hợp trong cùng một ứng dụng Micro-Prototype tương tác với luồng chuẩn:
1. **Common Context Header:** Hiển thị bài học Day 17 *"Finding & Validating Pain Points"* + 3 Snippets dữ liệu thật (Highlight, Note, Chưa hiểu).
2. **Option Switcher & Annotation Banner (Dành cho Facilitator/Reviewer):** Cho phép chuyển đổi linh hoạt giữa Option A, B, C và xem mục tiêu kỳ vọng kiểm tra của từng option.
3. **Critical Interaction Zone:**
   - **Option A:** Khay Snippets bên trái $\rightarrow$ Khung soạn Quiz kéo thả bên phải $\rightarrow$ Nút *"Lưu bộ Quiz thủ công"*.
   - **Option B:** Khung AI Suggestion Stream $\rightarrow$ 3 thẻ câu hỏi kèm Badge nguồn $\rightarrow$ Các nút thao tác *[Chấp nhận]* / *[Chỉnh sửa]* / *[Đổi câu hỏi khác]* $\rightarrow$ Nút *"Xác nhận & Bắt đầu luyện tập"*.
   - **Option C:** Dashboard Smart Study-Pack tự động $\rightarrow$ 5 câu hỏi phân hóa $\rightarrow$ Nút *"Bắt đầu làm Quiz ngay"* $\rightarrow$ Bảng điều khiển *[Độ khó]* & Nút *[Rollback về ghi chú thô]*.
4. **Result / Decision State & Reset Path:** Màn hình kết quả làm bài quiz hoặc thông báo hoàn tất bộ thẻ, kèm nút *"Reset về ngữ cảnh ban đầu"* để test lại.
