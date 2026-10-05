# Case B AI Notes — ba cách tạo ghi chú từ một bài học LLM

Đây là bài nộp cá nhân của **Nguyễn Thành Tiến — 2A202603003** cho lab thiết kế Human–AI. Tôi dùng cùng một bài học 94 slide để so sánh ba cách chia việc giữa người học và hệ thống: tự chọn nội dung, duyệt gợi ý, hoặc nhận ghi chú tự động. File [prototype.html](prototype.html) là bản có thể thao tác.

## 1. Thông tin bài làm

- Học viên: **Nguyễn Thành Tiến**, mã học viên **2A202603003**.
- Nhóm ở Day 17: **Bee**. Bài nộp này do một người phụ trách toàn bộ A/B/C.
- Case: **B — AI Notes: Personal Learning Notes**.
- Nội dung dùng chung: **Introduction to Large Language Models**, Lê Anh Cường, 8/2024, 94 trang.
- Bộ file tuân theo cấu trúc tối thiểu của tài liệu Day 19: README, Design Sheet, Prototype Link, Feedback Note, Synthesis và AI Support Log.

## 2. Hypothesis Problem và dấu vết Day 17

**Khi vừa học xong một bài dài**, học viên gặp khó khăn trong việc **giữ lại và sắp xếp những ý cần ôn** vì ít ghi chú hoặc chỉ lưu các liên kết rời rạc, dẫn đến **phải xem lại nhiều trang và tốn thời gian tra cứu**. Trong Interview Record Day 17, người tham gia kể rằng họ thường lưu link bài hữu ích, ít ghi chú và tra cứu lại khi gặp phần khó. Đây là đầu vào cho giả thuyết, không phải kết luận rằng mọi học viên đều gặp cùng vấn đề. [Design Sheet](three-option-design-sheet.md) tách lời kể, diễn giải và điểm cần kiểm tra.

## 3. Three Solution Options và prototype

| Option | Cơ chế | Quyền quyết định trước khi có ghi chú |
| --- | --- | --- |
| [A — Tôi chọn trước](prototype.html?option=A) | Đánh dấu slide **Giữ** hoặc **Chưa hiểu**, rồi yêu cầu tổng hợp. | Người học quyết định nội dung đầu vào. |
| [B — AI gợi ý trước](prototype.html?option=B) | Xem bốn gợi ý, giữ ý phù hợp hoặc thêm slide bị bỏ sót, rồi tạo ghi chú. | Người học duyệt đề xuất trước khi hệ thống soạn. |
| [C — AI tự tạo ngay](prototype.html?option=C) | Mở C là ghi chú xuất hiện từ chữ đã trích của bài PDF mẫu. | Hệ thống khởi tạo; người học đối chiếu và quyết định lưu. |

Giao diện gồm **cột trái chọn A/B/C, cột giữa xem slide, cột phải xem ghi chú**. Cả ba dùng cùng PDF, cùng mục tiêu tạo một ghi chú có thể tìm lại nguồn. Ở mỗi cách, người học có thể mở slide nguồn, sửa, bỏ hoặc xác nhận lưu ghi chú; nút **Đặt lại bài thử** đưa về trạng thái ban đầu.

**Cách mở:** giải nén đủ bộ file, giữ `prototype.html`, `Introduction-to-LLMs.pdf` và `lesson-slides/` cạnh nhau, rồi mở HTML trong Google Chrome. Xem [prototype-link.md](prototype-link.md) để thử từng option. Đây là prototype HTML chạy trên máy. Phần tạo ghi chú dùng quy tắc và dữ liệu mẫu đã xử lý từ PDF, không gọi mô hình AI trực tuyến. Ghi chú chỉ được lưu trong Chrome sau khi bấm **Xác nhận và lưu**.

## 4. Đóng góp của tôi

Tôi giữ Case B từ Day 17, chốt cùng một vấn đề và một bài học để so sánh ba cơ chế. Tôi quyết định bố cục ba cột, cách người học lấy lại quyền kiểm soát, và nội dung cần hiện trong ghi chú: ý muốn nhớ, chỗ cần tìm hiểu thêm, ghi chú cá nhân và trang nguồn. Tôi rà luồng A/B/C, thao tác quay về nguồn, sửa, bỏ, lưu và đặt lại. AI được dùng để triển khai mã, xử lý PDF mẫu, tạo slide trình bày và hỗ trợ biên tập; phạm vi được ghi trong [AI Support Log](ai-support-log.md).

## 5. Prototype Feedback và Next Change

[Feedback Note](prototype-feedback-note.md) ghi **một lượt kiểm thử A/B/C** trên cùng bài học, theo trình tự thao tác, điểm vướng và cách phục hồi. [Group Feedback Synthesis](group-feedback-synthesis.md) so sánh ba cơ chế trong lượt đó và chốt **một thay đổi tiếp theo**: đọc được nhiều hơn từ các slide có hình hoặc sơ đồ trước khi mở rộng cách C. Điểm vẫn cần kiểm tra ở vòng sử dụng tiếp theo là người học có đối chiếu trang nguồn và thấy ghi chú đủ hữu ích khi ôn bài thật hay không.

## 6. AI Support Log

[AI Support Log](ai-support-log.md) nêu cụ thể việc AI hỗ trợ, đầu ra được giữ, lỗi/giới hạn được sửa trong prototype và phạm vi của phần mô phỏng.
