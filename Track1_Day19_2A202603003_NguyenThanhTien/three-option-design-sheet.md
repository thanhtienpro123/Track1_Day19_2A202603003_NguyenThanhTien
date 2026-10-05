# Three Option Design Sheet — Case B AI Notes

**Người thực hiện:** Nguyễn Thành Tiến · **Bài học thử:** Introduction to Large Language Models, 94 slide · **Kết quả cần đạt:** một ghi chú ngắn có thể sửa và truy về trang nguồn.

## Chặng 1 — Evidence Snapshot và Hypothesis Problem

**Nguồn evidence duy nhất: Interview Record Day 17.** Người tham gia kể rằng họ không thường ghi chú hoặc highlight; khi gặp bài hữu ích, họ lưu link để tìm lại. Với phần khó, họ tiếp tục nghe giảng rồi tự tra cứu; khi ôn, họ nghe lại bài và dùng các link đã lưu. Họ nói đọc một lần dễ quên và tra cứu kiến thức khó tốn thời gian. Tôi hiểu từ cuộc trò chuyện này rằng một ghi chú ngắn, có mục cho phần chưa hiểu và có đường về bài gốc **có thể** giúp việc ôn thuận tiện hơn.

**Hypothesis Problem:** Khi vừa học xong một bài có nhiều ý cần nhớ, **học viên** gặp khó khăn trong việc **giữ lại và sắp xếp những điều quan trọng để ôn** vì họ ít ghi chú hoặc dấu vết chỉ nằm ở các link rời rạc, dẫn đến **phải xem lại nhiều trang và tốn thời gian tra cứu**.

**Điểm cần kiểm tra:** mức độ thường xuyên của khó khăn, việc người học có mở lại ghi chú khi ôn, và liệu họ muốn tự chọn nội dung hay chấp nhận ghi chú hệ thống tạo trước. PDF LLM là nội dung thử chung, không phải tài liệu người tham gia Day 17 đã dùng trong cuộc phỏng vấn.

## Chặng 2 — Từ Solution Parking Lot đến ba cơ chế

Parking Lot Day 17 gồm: mẫu ghi chú tự điền, link tài nguyên liên quan, checklist ôn tập, tìm kiếm trong bài/ghi chú cũ, và AI gợi nhóm nội dung. Tôi giữ hướng người học tự chọn cho A, phát triển hướng AI gợi ý cho B, và thêm hướng AI chủ động tạo ghi chú cho C. Liên kết trang nguồn được dùng chung ở cả ba.

### Comparison Contract

| Thành phần giữ nguyên | Quyết định chung cho A/B/C |
| --- | --- |
| Target user | Học viên vừa học một bài dài về LLM. |
| Situation | Cần giữ lại kiến thức để ôn sau bài. |
| Task | Tạo một ghi chú ngắn về bài học. |
| Desired outcome | Ghi chú có ý quan trọng, chỗ cần tìm hiểu thêm, phần cá nhân và trang nguồn; chỉ lưu khi người học xác nhận. |
| Content/data fixture | PDF 94 trang, cùng ảnh slide, cùng bộ chữ trích, cùng bố cục ba cột. |

| Quyết định | A — Tôi chọn trước | B — AI gợi ý trước | C — AI tự tạo ngay |
| --- | --- | --- | --- |
| Solution mechanism | Người học đánh dấu slide rồi hệ thống sắp xếp. | Hệ thống gợi bốn chủ đề, người học duyệt hoặc bổ sung trước khi tạo. | Hệ thống tự soạn một bản sáu chủ đề khi mở C. |
| User làm gì? | Chọn **Giữ** hoặc **Chưa hiểu**, yêu cầu tổng hợp, sửa và lưu. | Giữ/bỏ gợi ý, thêm slide, tạo ghi chú, sửa và lưu. | Đọc bản nháp, mở nguồn, sửa/bỏ/tạo lại rồi quyết định lưu. |
| Hệ thống làm gì? | Tóm tắt phần đã chọn; không tự thêm slide khác. | Đề xuất và tổng hợp những mục đã được duyệt. | Quét nội dung chữ từ bài mẫu và dựng ghi chú ngay. |
| Trigger | Nút **Tổng hợp slide đã chọn**. | Nút **Tạo ghi chú từ mục đã duyệt**. | Hành động mở C. |
| Trade-off | Sát ý cá nhân nhưng tốn công chọn. | Vào việc nhanh, vẫn có bước duyệt nhưng có thể bỏ sót. | Nhanh nhất, song cần kiểm tra kỹ hình và sơ đồ. |

**Distance check:** A khác B ở nguồn chọn nội dung đầu tiên. B khác C ở bước người học duyệt trước khi soạn. A khác C ở chỗ C chủ động tạo bản nháp từ toàn bài, còn A chỉ xử lý những slide người học đã chỉ định.

## Chặng 3 — Human–AI Design pass

| Quyết định Human–AI | A | B | C |
| --- | --- | --- | --- |
| Expectation | Giao diện nói rõ cần đánh dấu trang rồi mới tổng hợp. | Giao diện hiện các gợi ý và trang nguồn trước nút tạo. | Giao diện báo ghi chú tự xuất hiện từ chữ trích của PDF mẫu. |
| Role & Agency | Hệ thống **Ask**: chờ người học chọn và bấm tạo. | Hệ thống **Ask**: gợi ý trước, chờ duyệt. | Hệ thống **Act**: tạo nháp khi mở C; **không tự lưu**. |
| Evidence & Uncertainty | Ghi chú chỉ ra slide đã chọn; slide chủ yếu là hình cần xem trực tiếp. | Từng gợi ý có trang nguồn; có nút thêm slide bị bỏ sót. | Mỗi ý có trang nguồn; thông báo việc chữ trong hình/sơ đồ có thể chưa được bao quát. |
| Control & Recovery | Bỏ chọn, tổng hợp lại, sửa, bỏ hoặc lưu nháp. | Bỏ gợi ý, thêm trang, tạo lại, sửa, bỏ hoặc lưu. | Mở nguồn, sửa, bỏ, tạo lại hoặc lưu; bản tự tạo không được ghi vào bộ nhớ khi chưa xác nhận. |
| Nếu sai, người học mất gì? | Có thể mất thời gian chọn lại; bản đã lưu chỉ đổi khi bấm xác nhận. | Có thể thiếu một chủ đề; bổ sung trang rồi tạo lại. | Có thể hiểu nhầm bản tự tạo đã đủ; cần nhìn nguồn trước khi lưu. |

**Dữ liệu và phản hồi:** Prototype dùng bộ chữ đã trích sẵn từ PDF mẫu. Nội dung người học sửa chỉ nằm trong trình duyệt hiện tại; nút **Xác nhận và lưu** dùng localStorage, còn **Đặt lại bài thử** xóa ghi chú A/B/C. Không có luồng tải tài liệu hoặc ghi chú lên dịch vụ bên ngoài. Không có cơ chế học từ phản hồi ở các lần dùng sau.

## Chặng 4 — Ba micro-prototype có thể thử

| Trạng thái | A | B | C |
| --- | --- | --- | --- |
| Common context | Cùng bài LLM, xem slide ở giữa, chọn cách ở bên trái. | Cùng như A. | Cùng như A. |
| Critical interaction | Đánh dấu **Giữ/Chưa hiểu** trên slide 6 và 14. | Giữ gợi ý về mô hình ngôn ngữ; thêm slide 83 nếu thấy AI bỏ sót. | Mở C và đọc bản nháp tự xuất hiện. |
| Result/decision | Đối chiếu trang nguồn, sửa và lưu/bỏ. | Đối chiếu trang nguồn, sửa và lưu/bỏ. | Đối chiếu sáu chủ đề với slide nguồn, sửa và lưu/bỏ. |

File [prototype.html](prototype.html) chứa ba luồng trong một giao diện. Cột trái là ba cơ chế, cột giữa là ảnh của 94 trang PDF, cột phải là gợi ý hoặc ghi chú. Nút trên ghi chú nhảy về slide nguồn. Để reset về ngữ cảnh chung, dùng nút **Đặt lại bài thử** ở đầu trang.

**Prototype annotations — ngoài màn hình thử:**

| Option | Tôi kỳ vọng người thử làm | Quan sát | Không giải thích hộ |
| --- | --- | --- | --- |
| A | Tự tìm slide muốn giữ, đánh dấu, rồi tổng hợp. | Có nhận ra **Chưa hiểu** khác **Giữ** không; có kiểm tra nguồn không. | Nút nào nên bấm đầu tiên. |
| B | Xem gợi ý, giữ một ý, thêm một trang không nằm trong gợi ý. | Có thấy đường thêm trang và hiểu gợi ý chưa phải ghi chú cuối không. | AI đã chọn đúng hay sai. |
| C | Nhận ra ghi chú đã hiện, mở nguồn và quyết định sửa/lưu. | Có tưởng ghi chú đã lưu chưa; có kiểm tra sơ đồ không. | Nội dung nào là quan trọng nhất. |

## Chặng 5 — Test prompt và observation focus

**Relevant context:** “Gần đây bạn đã lưu hoặc ghi lại nội dung học để xem lại như thế nào?”

**Outcome task dùng nguyên văn cho A/B/C:** “Bạn vừa học xong bài Introduction to LLMs. Hãy dùng từng cách để tạo một ghi chú bạn sẽ muốn giữ lại khi ôn. Bạn có thể sửa nội dung nếu thấy chưa đúng với ý mình.”

**Quan sát tối đa năm điểm:** thao tác đầu tiên; chỗ dừng hoặc hiểu sai; có mở nguồn hay bỏ qua; cách sửa/bỏ/lưu; phương án chọn và đánh đổi được nêu. Người điều phối chỉ giao nhiệm vụ, để người thử tự bấm và không hỏi “Bạn có thích không?”. Nếu họ dừng, dùng câu trung tính: “Bạn sẽ làm gì tiếp theo?”

## Chặng 6 — Feedback và một Next Change

[Prototype Feedback Note](prototype-feedback-note.md) ghi **một lượt chạy cả A/B/C**, với thao tác và diễn giải tách riêng. [Group Feedback Synthesis](group-feedback-synthesis.md) so sánh ba cơ chế trong lượt đó để thấy trade-off. Quyết định cho vòng sau là **cải thiện việc nhận nội dung trong hình/sơ đồ của PDF trước khi mở C cho bài khác**, vì hiện C chỉ dùng chữ trích. Điều chưa chứng minh là người học có dùng ghi chú này khi ôn thật và chấp nhận mức độ tự động nào.
