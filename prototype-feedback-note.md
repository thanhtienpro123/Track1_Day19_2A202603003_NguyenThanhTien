# Prototype Feedback Note — ba lượt kiểm thử Case B AI Notes

**Người ghi:** Nguyễn Thành Tiến · **Nội dung thử:** cùng bài Introduction to LLMs 94 slide · **Nhiệm vụ:** tạo một ghi chú muốn giữ lại để ôn, đối chiếu nguồn và sửa chỗ chưa đúng. Ba lượt dưới đây là **kiểm thử kịch bản trên prototype**, ghi thao tác và kết quả của giao diện; các nhận định về người học được đặt riêng trong phần diễn giải.

## Cách tiến hành

Mỗi lượt bắt đầu bằng **Đặt lại bài thử**, dùng đủ A/B/C và cùng mục tiêu tạo ghi chú. Tôi nhìn vào thao tác đầu tiên, chỗ cần dừng để kiểm tra, việc mở nguồn, cách sửa/lưu/bỏ và đánh đổi của từng cơ chế. Tôi không dùng câu “thích hay không” làm tiêu chí. Các kịch bản đại diện cho ba nhu cầu: nhớ khái niệm, làm rõ chỗ chưa hiểu và ôn phần kỹ thuật.

## Feedback 1 — Giữ khái niệm nền tảng

**Bối cảnh thử:** vừa học xong phần mở đầu về mô hình ngôn ngữ; muốn lưu định nghĩa và cách huấn luyện.

| Observation | Ghi nhận thao tác trên prototype |
| --- | --- |
| First action | Ở A, nhập trang 6 và bấm **Giữ trang này**. Ở B, xem gợi ý **Mô hình ngôn ngữ**. Ở C, mở tab là ghi chú hiện ngay. |
| Dừng hoặc hiểu sai | A phải chuyển tới đúng slide mới đánh dấu được. B có hai lớp quyết định: giữ gợi ý rồi mới tạo. C không có bước khởi tạo nên cần nhìn trạng thái **Chưa lưu**. |
| Evidence được đọc | Ghi chú A có nguồn trang 6; B ghi nguồn trang 6 và 9; C có nút nguồn cho từng nhóm nội dung. |
| Sửa hoặc lấy lại control | A có thể đổi slide đã chọn và tổng hợp lại. B có thể bỏ gợi ý. C có thể sửa trực tiếp trước khi lưu. |
| Đánh đổi của lượt thử | A sát đúng trang tôi chọn nhưng nhiều thao tác hơn; B giúp bắt đầu nhanh; C tạo bản bao quát hơn nhu cầu chỉ lưu một khái niệm. |

**Observed:** A chỉ đưa slide đã đánh dấu vào ghi chú; B không tự tạo trước khi bấm nút; C tự hiện nháp mà chưa ghi vào bộ nhớ. **Interpreted:** với nhu cầu rất hẹp, A có lợi thế kiểm soát, còn C dễ tạo nhiều ý cần lọc. **Decided — next change:** giữ nút nguồn rõ ràng và trạng thái lưu ở cả ba. **Still unproven:** người học sẽ chọn mức độ chủ động nào cho một bài học của chính họ.

## Feedback 2 — Ghi lại phần chưa hiểu

**Bối cảnh thử:** muốn nhớ ba chặng huấn luyện ChatGPT và đánh dấu một điểm để đọc lại.

| Observation | Ghi nhận thao tác trên prototype |
| --- | --- |
| First action | Ở A, tới trang 14 và chọn **Chưa hiểu trang này**. Ở B, giữ gợi ý **Huấn luyện ChatGPT**. Ở C, đọc mục **Điều cần tìm hiểu thêm** đã được tạo sẵn. |
| Dừng hoặc hiểu sai | A phân biệt được **Giữ** với **Chưa hiểu**, nhưng nháp chỉ xuất hiện sau nút tổng hợp. B cho xem gợi ý nhưng chưa biết điều người học thắc mắc nếu họ không thêm trang. C đặt sẵn câu hỏi về zero-shot/few-shot và PPO/DPO; cần sửa theo nhu cầu cá nhân. |
| Evidence được đọc | A dẫn về trang 14; B dẫn về trang 14 và 18; C có nguồn trang 27 và 55 cho phần cần xem lại. |
| Sửa hoặc lấy lại control | Có thể sửa mục **Điều cần tìm hiểu thêm** ở cả ba. C cho bỏ bản nháp và tạo lại; sau khi bỏ, chuyển tab qua lại không tự tạo lại ngoài ý muốn. |
| Đánh đổi của lượt thử | A ghi chính xác điểm chưa hiểu nhưng yêu cầu tự đánh dấu; B giúp chọn chủ đề; C đặt câu hỏi sẵn nhanh nhưng có thể lệch thắc mắc thật. |

**Observed:** mục **Chưa hiểu** của A vào đúng phần ghi chú riêng; C cho sửa, bỏ và tạo lại. **Interpreted:** phần “cần tìm hiểu thêm” nên xuất phát từ dấu vết của người học khi có sẵn, thay vì luôn dùng câu hỏi mẫu. **Decided — next change:** giữ phần này có thể sửa ngay trước khi lưu. **Still unproven:** câu hỏi gợi ra từ bài có giúp người học ôn tốt hơn câu hỏi họ tự viết hay không.

## Feedback 3 — Kiểm tra một ý hệ thống dễ bỏ sót

**Bối cảnh thử:** muốn ôn phần kỹ thuật ở cuối bài, đặc biệt là knowledge distillation ở trang 83–84.

| Observation | Ghi nhận thao tác trên prototype |
| --- | --- |
| First action | Ở A, tới trang 83 và chọn **Giữ trang này**. Ở B, thấy bốn gợi ý không có distillation, tới trang 83 và bấm **Thêm trang này vào B**. Ở C, distillation đã nằm trong ghi chú tự động. |
| Dừng hoặc hiểu sai | B cần người học nhìn cả cột giữa và cột phải để nhận ra đường bổ sung. C có vẻ đầy đủ với chủ đề này nhưng cần kiểm tra các slide nhiều hình khác. |
| Evidence được đọc | Ghi chú B sau khi tạo có trang 83; C có nguồn trang 83–84. Nút nguồn đưa cột giữa về đúng trang tương ứng. |
| Sửa hoặc lấy lại control | B có thể bỏ trang đã thêm hoặc tạo lại sau khi đổi lựa chọn. C có thể sửa, bỏ nháp; chỉ bấm **Xác nhận và lưu** mới lưu. |
| Đánh đổi của lượt thử | B vừa nhanh vừa cho bổ sung ý thiếu, nhưng thao tác thêm trang có thể bị bỏ qua. C bao quát nhiều chủ đề, song chữ nằm trong sơ đồ của PDF không được đọc đầy đủ. |

**Observed:** B nhận được trang 83 do người học thêm; C tự đưa chủ đề distillation vào ghi chú và có nguồn để đối chiếu. **Interpreted:** đường bổ sung của B xử lý được một kiểu bỏ sót, còn chất lượng C phụ thuộc vào phần chữ trích từ PDF. **Decided — next change:** ưu tiên cải thiện nội dung lấy từ slide hình/sơ đồ trước khi mở rộng C. **Still unproven:** ghi chú tự động có đủ đúng và đủ ngắn đối với một người học đang ôn thật hay không.

## Kết luận của người rà prototype

Ba cơ chế tạo ra ba thời điểm quyết định khác nhau: **A chọn trước**, **B duyệt giữa chừng**, **C kiểm tra sau**. Cả ba có cùng nơi xem bài, cùng cấu trúc note và cùng đường về nguồn. Điểm mạnh rõ trong lượt kiểm thử là khả năng sửa/bỏ/lưu có chủ đích; điểm cần cải thiện là độ bao phủ nội dung trong hình và sơ đồ của bài PDF. Tôi dùng ba lượt này làm input cho [bản tổng hợp](group-feedback-synthesis.md), không dùng chúng như số liệu chứng minh giá trị sản phẩm.
