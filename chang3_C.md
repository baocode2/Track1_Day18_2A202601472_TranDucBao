# Chặng 3 — Human–AI Decision Table (Cột C: Trần Đức Bảo)

**Nhóm:** cuong
**Case B** — AI Notes: Personal Learning Notes
**Option phụ trách:** Option C — *Autonomous Study Digest & Mini-Quiz (AI-Led, Act with Guardrails & Instant Rollback)*

> Bản nháp — chỉ điền cột C theo phân công (Bảo phụ trách Option C, xem
> [02-three-solution-options.md](02-three-solution-options.md)). Căn cứ trên evidence và
> Hypothesis Problem đã chốt ở [01-evidence-huddle.md](01-evidence-huddle.md). Để đọc và
> hiệu chỉnh lại trước khi gộp vào bảng chung ba cột A/B/C.

| Human–AI decision | Option C |
|---|---|
| **User làm gì? AI làm gì?** | **User:** mở trang ôn tập → nhận ngay bản digest hoàn chỉnh (3 ý cốt lõi + 1 mục giải thích điểm khó + 3 câu trắc nghiệm), đọc hoặc làm quiz ngay; có thể bấm *"Tùy chỉnh theo mục tiêu"* hoặc *"Rollback về ghi chú thô"* nếu không ưng.<br>**AI:** tự động phân tích trọn 3 snippet (highlight Slide 3, note Slide 7, ảnh "Chưa hiểu" Slide 11) và sinh 100% nội dung ngay khi trang tải — không chờ user xác nhận trước. Gộp cả hai nhu cầu đã thấy ở huddle: giải thích điểm khó (nhu cầu của Hoàn, #1) và bộ câu hỏi tự kiểm tra (nhu cầu của Mai, #5). |
| **AI Act / Ask / Don't Act? Vì sao?** | **Act (with Guardrails).** Chọn Act vì mục tiêu của option này là loại bỏ hoàn toàn chi phí tổng hợp thủ công — đúng pattern nghẽn nhóm xác định là lặp ở cả hai nguồn (khâu *chuyển đổi* note thô, không phải khâu ghi). Không chọn Ask vì mỗi lượt hỏi-duyệt lại cộng thêm chi phí mà chính user (Mai, #5) đã gọi là *"tốn thời gian nhất"*. Nhưng vì đây là suy luận tự động trên nội dung học thuật — rủi ro tóm tắt sai ý hoặc quiz lệch trọng tâm — nên bắt buộc kèm guardrail: giữ nguyên bản gốc song song, cho rollback tức thì, không bao giờ tự ý ghi đè note gốc của user. |
| **User hiểu capability/limit bằng gì?** | Banner hiện ngay khi trang tải xong: *"Đã tạo bản tóm tắt và 3 câu hỏi trắc nghiệm dựa trên slide bài học"*. Cần nói rõ thêm giới hạn: đây là bản nháp do AI tổng hợp tự động từ đúng 3 snippet đã lưu, **không phải** xác nhận đúng/sai về kiến thức, và không suy luận thêm ngoài phạm vi 3 mẩu note đó. |
| **Evidence/uncertainty được thể hiện thế nào?** | Mỗi mục trong digest (ý cốt lõi / mục giải thích / từng câu quiz) gắn Source Citation + thumbnail của đúng slide gốc (Slide 3 / 7 / 11) để user đối chiếu ngay, không phải tin suông. Không hiển thị % độ tin cậy vì AI không suy luận ngoài input có sẵn — nhưng câu quiz là nội dung **sinh mới** (không trích nguyên văn như phần tóm tắt), nên cần thêm nhãn kiểu *"câu hỏi tự sinh, chưa qua duyệt"* để tách rõ với phần trích dẫn trực tiếp. |
| **User kiểm soát và recovery thế nào?** | Nút *"Khôi phục về ghi chú gốc"* (Instant Rollback) luôn hiện sẵn, phục hồi tức thì về đúng 3 snippet thô ban đầu — đây là guardrail bắt buộc chứ không phải tính năng phụ, vì Option C là option duy nhất không có bước duyệt trước khi hiển thị (khác Option B). Kèm nút *"Chỉnh sửa"* từng mục và nút *"Tùy chỉnh theo mục tiêu điểm"* (đổi độ khó/độ dài theo mục tiêu điểm — ứng với việc Hoàn chủ động bỏ bớt theo mục tiêu điểm, #3). |
| **Feedback and data check — khi liên quan** | Vì AI xử lý ngay ảnh chụp/ghi chú cá nhân của user, cần auto-save bản gốc *trước khi* AI xử lý (đối phó rủi ro mất file đã thấy ở #6 — Notepad thất lạc do quên Ctrl+S). Mỗi thẻ digest nên có nút *"Báo sai"* hoặc đánh giá nhanh để ghi nhận khi tóm tắt/quiz lệch ý, làm input cho vòng lặp sau. Đây vẫn là điểm mở, chưa có cam kết chính thức — Evidence Huddle chưa có nguồn nào cho hậu quả định lượng nếu digest sai, nên feedback loop này là hướng cần thử nghiệm thêm, không phải đã validated. |

---

**Việc còn mở khi hiệu chỉnh:**
- Row "Evidence/uncertainty" — cân nhắc có cần nhãn cảnh báo riêng cho phần quiz tự sinh hay để chung với phần tóm tắt.
- Row "Feedback and data check" — câu hỏi trong đề gốc bị cắt ở dấu `—`, cần đối chiếu lại nguyên văn đề bài trước khi chốt nội dung này.
