- Đức: tính năng hỏi đáp đang hơi chậm và bên cạnh đó nên thêm nút "?" để khi ấn vào hình ảnh thì có thể hỏi đáp luôn tại đó thay vì chụp ảnh như hiện tại
 <br>Người khảo sát: Trần Đức Bảo
---

## Mẫu ghi quan sát khi test

**Tester/context:** Đức (Bàn bên cạnh) - Nhờ test và cho xin feedback về sản phẩm

| Observation | Note |
|---|---|
| First action | User tự chụp ảnh và test các tính năng hỏi đáp có nối api realtime của nhóm |
| Chỗ dừng, do dự hoặc hiểu sai | User muốn cải thiện tính năng chụp ảnh bằng cách có trạng thái hỏi được bật thì di chuột vào các ô thắc mắc thì sẽ có context trả lời luôn |
| Evidence được đọc hay bỏ qua | Được đọc|
| Cách tester sửa hoặc lấy lại control | Đưa ra gợi í |
| Option được chọn | B |
| Lý do và trade-off | Vì B có thể kiểm soát luồng AI hoạt động một cách chủ động không bị làm phiền khi đã hiểu bài|
| Evidence chống lại kỳ vọng của nhóm | Nhóm nghĩ việc chụp ảnh sẽ giúp tăng tốc độ hỏi bài nhưng câu hỏi của user đã cho thấy việc chụp ảnh sẽ cho thời gian lâu hơn chế độ hỏi đáp và hover chuột đến |

---

## Đối chiếu ba lượt feedback

| Nội dung | Feedback 1 (Đức) | Feedback 2 | Feedback 3 | Pattern hoặc khác biệt |
|---|---|---|---|---|
| First action | Tự chụp ảnh, test hỏi đáp realtime |  |  | |
| Breakdown chính | Muốn hover để hỏi luôn thay vì phải chụp |  |  | |
| Cách lấy lại control | Chỉ góp ý bằng lời, không dùng nút sửa/rollback nào |  |  | |
| Option được chọn | B |  |  | |
| Trade-off | Chọn B để chủ động kiểm soát, không bị AI làm phiền khi đã hiểu bài |  |  | |

**Một Next Change nhóm chốt:** ..........................................................

**Evidence nào dẫn tới quyết định này:** ..........................................................

**Still Unproven sau ba feedback:** 

---

## AI Support Log — Trần Đức Bảo

**AI đã giúp tôi ở đâu?**
- Giúp định hướng hướng đi cho bài làm, giúp tôi viết những bằng chứng hay giả thuyết dài làm định hướng cho tôi nghiên cứu và phần tích user, hỗ trợ design làm ui cho giao diện demo

**AI sai, hời hợt hoặc làm các options giống nhau ở đâu?**
- Làm chưa đúng những thông tin yêu cầu và bị trùng lặp các option về suy luận logic, AI vẫn chưa thể phân tích dược hypothesis problem chính xác, phân tích logic các solution chưa được chi tiết

**Tôi đã tự sửa hoặc quyết định lại điều gì?**
- Tự sửa logic của các đoạn chat, tự suy luân những hành vi có thể xảy ra từ envidence và nghiên cứu suy ra được, bên cạnh đó quyết định model call api, quyết định cấu trúc file nộp và xác định sự thật cho AI thực hiện

---
