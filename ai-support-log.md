# AI Support Log — Case B AI Notes

Tôi dùng AI như công cụ hỗ trợ phân tích đề, triển khai prototype và rà lỗi. Tôi giữ quyết định thiết kế dựa trên cùng một Hypothesis Problem và cùng bài học LLM để ba option có thể so sánh.

| Công đoạn | AI hỗ trợ cụ thể | Tôi giữ hoặc sửa trong bài |
| --- | --- | --- |
| Đọc yêu cầu | Rút ra sáu chặng, năm gate và cấu trúc sáu file nộp từ Day 19/checklist. | Giữ một problem của Case B, cùng task và cùng PDF cho A/B/C. |
| Chọn cơ chế | Gợi spectrum người học chọn → duyệt gợi ý → hệ thống tự tạo. | Chốt A chọn slide trước, B duyệt gợi ý trước, C tự tạo note khi mở. Ba cách khác ở thời điểm quyết định, không chỉ ở giao diện. |
| Tạo dữ liệu mẫu | Trích phần chữ và tạo 94 ảnh slide từ PDF Introduction to LLMs. | Dùng cùng một bài học; mỗi ý trong ghi chú có số trang để người học kiểm tra. |
| Viết mã | Hỗ trợ HTML/CSS/JavaScript cho bố cục ba cột, các nút chọn slide, gợi ý, tạo nháp, sửa, lưu và đặt lại. | Giữ thao tác Chrome offline, font tiếng Việt Be Vietnam Pro, và không tự lưu ghi chú C. |
| Trình bày | Tạo một slide PowerPoint minh họa giao diện. | Dùng PPTX để thuyết trình, HTML để thao tác thật. |
| Rà sản phẩm | Kiểm tra các luồng A/B/C, nguồn, chỉnh sửa, lưu, bỏ, tạo lại và reset. | Bổ sung đường **Thêm trang này vào B** để người học sửa trường hợp AI gợi thiếu. |
| Viết báo cáo | Hỗ trợ sắp xếp Design Sheet, Feedback Note và bản tổng hợp. | Giữ tách biệt lời kể Day 17, kết quả kiểm thử giao diện và diễn giải của tôi. |

## Lỗi và giới hạn tôi nhận ra khi rà lại

Ban đầu C được hiểu như “AI tự đọc PDF” ở mọi lần chạy. Cách gọi đó quá rộng so với bản mẫu: nội dung chữ của **PDF này** đã được xử lý trước và đóng gói trong HTML; JavaScript dùng quy tắc chọn sáu chủ đề để soạn ghi chú khi mở C. Tôi sửa cách mô tả trên giao diện và trong báo cáo để người dùng hiểu đúng điều đang xảy ra. Một số slide chứa hình hoặc sơ đồ có ít chữ trích được, nên ghi chú C cần đường mở trang nguồn và bước người học xác nhận trước khi lưu.

Tôi cũng xem lại B sau khi có gợi ý: nếu AI không nêu một chủ đề quan trọng, người học cần cách thêm slide ngay trong cùng luồng. Nút **Thêm trang này vào B** và **Tạo lại từ lựa chọn** giải quyết tình huống đó trong prototype.

## Điều tôi rút ra

Điểm cần so sánh không phải bản ghi chú nào dài hơn, mà là **ai khởi đầu việc chọn ý và người học lấy lại quyền quyết định ở đâu**. A đặt quyền chọn ở đầu, B đặt giữa quá trình, C đặt ở bước kiểm tra cuối. Giữ cùng PDF và cùng khung note làm khác biệt cơ chế rõ hơn. Với C, tốc độ có giá trị chỉ khi người học còn thấy được nguồn, sửa được ý sai và biết bản nháp chưa được lưu.

## Phạm vi sử dụng AI trong bản này

Prototype dùng quy tắc và canned output trên nội dung PDF mẫu, không có mô hình AI hay API trực tuyến. AI hỗ trợ viết và rà tài liệu; các lượt trong Feedback Note là thao tác kiểm thử kịch bản trên sản phẩm, không phải lời trích dẫn của người tham gia Day 17. Tài liệu phỏng vấn Day 17 được dùng đúng phạm vi như dấu vết khởi đầu cho giả thuyết.
