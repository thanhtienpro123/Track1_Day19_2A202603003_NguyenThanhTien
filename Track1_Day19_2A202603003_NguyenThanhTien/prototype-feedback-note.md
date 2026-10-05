# Prototype Feedback Note — một lượt thử A/B/C

**Người thử trong kịch bản:** T01, một học viên vừa học bài LLM. **Nội dung thử:** bài Introduction to LLMs, 94 slide. **Nhiệm vụ:** tạo một ghi chú về khái niệm mô hình ngôn ngữ, chỗ chưa hiểu trong quá trình huấn luyện và một ý ở cuối bài để ôn sau. Đây là **một lượt kiểm thử kịch bản trên prototype**. Các thao tác và kết quả giao diện được ghi trước; nhận xét thiết kế được đặt riêng bên dưới.

## Trình tự thao tác của một lượt thử

| Bước | Thao tác quan sát trên prototype | Kết quả hiển thị |
| --- | --- | --- |
| A — Tôi chọn trước | Mở trang 6, bấm **Giữ trang này**; đến trang 14, bấm **Chưa hiểu trang này**; bấm **Tổng hợp slide đã chọn**. | Ghi chú có ý từ trang 6, mục cần xem lại trang 14 và nút về hai trang nguồn. |
| B — AI gợi ý trước | Giữ gợi ý **Mô hình ngôn ngữ**; mở trang 83 và bấm **Thêm trang này vào B**; bấm **Tạo ghi chú từ mục đã duyệt**. | Ghi chú có cả ý được gợi và trang 83 được bổ sung trong lượt thử. |
| C — AI tự tạo ngay | Chuyển sang C, đọc ghi chú tự hiện; mở trang nguồn, sửa mục **Ghi chú của tôi**, rồi xem trạng thái trước khi lưu. | Ghi chú gồm sáu chủ đề và các trang nguồn; trạng thái vẫn là **Chưa lưu** cho tới khi bấm xác nhận. |

## Ghi nhận theo tiêu chí Day 19

| Observation | Ghi nhận của lượt thử |
| --- | --- |
| First action | A bắt đầu bằng chọn trang; B bắt đầu bằng xem gợi ý; C bắt đầu bằng đọc ghi chú đã có. |
| Chỗ dừng hoặc hiểu sai | A cần tìm đúng trang rồi mới đánh dấu. B cần nhìn cả cột gợi ý lẫn nút **Thêm trang này vào B** ở cột bài học. C dễ tạo cảm giác đã xong dù ghi chú chưa được đối chiếu. |
| Evidence được đọc | Cả ba cho quay về slide nguồn. Trang 83 được thêm vào B xuất hiện trong phần nguồn; C nêu trang nguồn cho các chủ đề tự tạo. |
| Sửa và lấy lại control | A đổi đánh dấu rồi tổng hợp lại được. B thêm/bỏ trang và tạo lại được. C cho sửa, bỏ bản nháp, tạo lại; không tự lưu. |
| Option phù hợp nhiệm vụ thử | **B** xử lý được cả ý hệ thống gợi và ý trang 83 cần bổ sung. Đây là lựa chọn cho kịch bản thử này, không phải kết luận về sở thích của người học nói chung. |
| Trade-off | A chính xác theo lựa chọn nhưng nhiều thao tác; B cân bằng gợi ý và bổ sung; C nhanh nhất nhưng cần rà kỹ nội dung lấy từ hình/sơ đồ. |
| Điều khác kỳ vọng | Gợi ý ban đầu của B không có distillation; phải thêm trang 83. C có distillation nhưng một số slide nhiều hình vẫn ít chữ trích được. |

## Tách quan sát, diễn giải và quyết định

**Observed:** trong một lượt thử, A tạo note từ trang 6 và 14 đã chọn; B nhận thêm trang 83 ngoài danh sách gợi ý; C tự hiện nháp và chưa lưu. Các nút nguồn, sửa, bỏ, tạo lại và xác nhận là đường để tiếp tục khi bản nháp chưa đúng.

**Interpreted:** A hợp khi người học biết rõ cần giữ trang nào. B hỗ trợ bắt đầu nhanh mà vẫn sửa được một trường hợp AI bỏ sót. C thuận tiện khi muốn có bản toàn bài, nhưng cách tạo từ chữ trích khiến phần hình/sơ đồ cần được kiểm tra trực tiếp.

**Decided — Next Change:** ưu tiên lấy thêm nội dung trong hình/sơ đồ và rà lại cách C tạo ghi chú, vì bản nháp tự động có thể trông đầy đủ hơn lượng thông tin thực sự đọc được.

**Still Unproven:** một lượt kiểm thử prototype chưa cho biết người học có dùng ghi chú này khi ôn bài thật hoặc sẽ chọn B trong tình huống của họ.
