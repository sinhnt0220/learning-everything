# Bộ định tuyến theo loại năng lực

Định tuyến từng phase/module theo performance cần tạo, không theo tên môn. Một khóa học thường trộn nhiều loại.

Định tuyến domain trước để chọn loại performance/evidence, sau đó dùng `lesson-depth.md` để chọn `MICRO | STANDARD | DEEP`. Domain route và depth route là hai quyết định khác nhau.

| Loại | Dạy ưu tiên | Independent Proof | Evidence/tool |
|---|---|---|---|
| Khái niệm | Định nghĩa, ranh giới, cơ chế, ví dụ/phản ví dụ | Phân biệt case gần nhau hoặc giải thích cơ chế trong biến thể | Sơ đồ, case, lập luận |
| Thủ tục/kỹ thuật | Demo chạy thật → guided modification → independent build/debug | Thực thi, sửa lỗi, thay requirement | Code, thao tác, test, artifact |
| Định lượng | Đại lượng, đơn vị, assumptions, worked calculation | Tính, kiểm tra và diễn giải | Phép tính, bảng, code |
| Thực nghiệm | Giả thuyết, biến, protocol, sai số, an toàn | Thiết kế/diễn giải thí nghiệm | Dữ liệu, mô phỏng, protocol; lab cần external validation |
| Dữ liệu | Câu hỏi, data quality, metric, uncertainty | Phân tích dataset và bảo vệ kết luận | Notebook, query, chart, log |
| Ra quyết định | Case, option, trade-off, risk, evidence | Chọn và nêu điều kiện đổi quyết định | Decision memo, scenario |
| Hệ thống | Boundary, variable, stock/flow, feedback, delay | Xây và phản biện mô hình/intervention | CLD, stock-flow, counterexample |
| Khoa học xã hội | Construct, observation, method, competing explanation, ethics | Audit claim/case với bằng chứng cạnh tranh | Paper, case, source matrix |
| Lịch sử/nhân văn | Provenance, bối cảnh, nguồn, diễn giải cạnh tranh | Bảo vệ cách đọc và mức chắc chắn | Primary/secondary sources |
| Sáng tạo | Exemplar, kỹ thuật, artifact, critique, revision | Tạo/sửa artifact theo brief | Draft, design, media, revision |
| Product/tool | Product map → demo → practice ladder → operate | Modification/debug/build có evidence | UI, export, execution log, render |

## Điều chỉnh theo nền

### Chưa có schema

- Không ép Socratic hoặc quiz thuật ngữ.
- Orientation ngắn và worked example/demo trước.
- Giao guided action gần ví dụ.

### Có nền

- Mở bằng artifact/case/lỗi thật.
- Dùng challenge phân giải để khóa baseline.
- Yêu cầu cơ chế, lựa chọn và điểm chưa chắc.

### Nâng cao

- Dùng case mơ hồ, boundary mới, trade-off, debugging và phản ví dụ.
- Yêu cầu nguồn gốc và bảo vệ quyết định.

## Domain Contract bắt buộc

Trước curriculum, xác định:

- Performance đích.
- Tiêu chuẩn đúng/sai.
- Bằng chứng hợp lệ.
- Source hierarchy.
- Misconceptions/failure modes.
- Safety/ethics/financial/privacy boundary.
- Tool/environment.
- External validation.

## Mẫu định tuyến

### Python/Computer Science

Trộn khái niệm + kỹ thuật. Mental model hỗ trợ việc chạy, sửa và thiết kế chương trình; PASS thực hành cần code chạy/test. Chọn nhánh automation/data/backend/AI application theo mục tiêu, không dạy toàn bộ CS trước khi tạo artifact.

### Psychology

Trộn khái niệm + khoa học xã hội + thực nghiệm + định lượng + ethics. Không thu hẹp toàn khóa thành critical thinking; mỗi module phải neo vào construct/cơ chế tâm lý cụ thể (ví dụ attribution, attention, learning, memory, motivation hoặc social influence), phương pháp nghiên cứu và giới hạn ứng dụng. “Quan sát khác diễn giải” chỉ đủ là Psychology khi được nối với cơ chế/construct tâm lý và bằng chứng liên quan. Không chẩn đoán từ case ngắn.

### Food Technology

Trộn hóa/sinh học + định lượng + thực nghiệm + process + regulation. Tùy module có thể là formulation, microbiology, unit operation, sensory, shelf life hoặc QA. Luôn xét đơn vị, protocol, an toàn và tiêu chuẩn hiện hành; không công nhận lab/production từ chat.

### Data Science

Trộn dữ liệu + định lượng + kỹ thuật + decision. Placement phải phân biệt năng lực lập luận dữ liệu với fluency của spreadsheet/SQL/Python; một năng lực không tự chứng minh năng lực còn lại. Đưa dataset nhỏ vào sớm. Capstone cần artifact tái lập và decision memo, không chỉ model score.

### Systems Thinking

Trộn hệ thống + khái niệm + decision. Chấm boundary, variable, causal claim, feedback, delay, assumption, counterexample và intervention; không chấm độ đẹp sơ đồ hoặc Permanent Note.

### Automation/AI tools

Trộn product/tool + kỹ thuật + decision; với media thêm sáng tạo. Dùng `product-practice.md`, tài liệu chính thức hiện hành, artifact thật và permission boundary.
