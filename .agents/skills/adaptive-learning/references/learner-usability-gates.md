# Learner usability gates

Áp dụng trước khi tạo hoặc sửa bất kỳ module/bài đọc learner-facing nào.

## 1. Phân biệt hai loại artifact

- **Artifact nội bộ của agent:** learning map, evidence ledger, task map chi tiết, rubric, state. Nó giúp Codex điều phối; learner không phải biết tên, mở hoặc gọi nó.
- **Artifact learner-facing:** một bài đọc, demo, checklist, trace hoặc output mà learner cần dùng để hiểu hay làm việc.

Không đưa artifact nội bộ thành “bài học” chỉ vì nó đúng cấu trúc.

### Hợp đồng lưu trữ

- `modules/*.md` là learner-facing.
- `learning-map.md` và `work/evidence-log.md` là nội bộ.
- Không đưa các heading như `Readiness Gate`, `Evidence stage`, `Permission/cost audit`, `Bài làm và artifact`, `Đánh giá` hoặc `Context handoff` vào module learner-facing.
- Không append nguyên văn bài làm, lịch sử chấm hoặc next pointer vận hành vào bài học.
- Nếu có rủi ro thật, chỉ đặt boundary ngắn ngay cạnh hành động có rủi ro; chi tiết audit ở lớp nội bộ.

QA/readiness vẫn phải được thực hiện trước khi bàn giao, nhưng “đã chạy gate” không phải nội dung người học cần đọc.

## 2. Gate trước khi bàn giao một bài đọc

Đầu bài phải trả lời bằng ngôn ngữ thường bốn câu:

1. Việc này giúp người học làm được gì?
2. Khi nào cần dùng, và khi nào không cần dùng?
3. Người học có phải mở file, gọi command hay tạo artifact nào không?
4. Hành động tiếp theo chính xác là gì?

Nếu một câu chưa rõ, chưa bàn giao bài.

Mỗi thuật ngữ mới được giữ lại phải có, theo thứ tự:

1. Một vấn đề hoặc tình huống sử dụng đủ để định vị.
2. Cơ chế/ranh giới bằng lời thường.
3. Tên thuật ngữ.
4. Một phản ví dụ hoặc điều kiện không cần dùng khi cần.

Không giới thiệu hai artifact nội bộ cùng lúc trừ khi case thật bắt buộc phải đối chiếu cả hai.

Không bắt buộc có worked trace trước cold attempt nếu learner đã có prerequisite liên quan. “Dạy trước” nghĩa là learner có theory cần thiết, không phải được xem trước cách giải.

## 3. Gate cho demo và evidence stage

- Static diagram, file tồn tại, hoặc danh sách định nghĩa không phải worked demo.
- Worked demo phải cho thấy input → hành động/quyết định → output → lý do của bước quan trọng.
- `MODELED` chỉ được ghi khi learner đã quan sát được trace hoàn chỉnh và nói được công dụng thực tế của nó. File có cấu trúc không đủ.
- Learner nói “tôi không hiểu” là bằng chứng mâu thuẫn: hạ state xuống `REVISE`/`INTRODUCED`; dừng mở bài mới.

## 4. Gate chống dẫn đường

Với task dự kiến đo `INDEPENDENT` hoặc `TRANSFER`:

- Giao một output thực tế, không dùng chuỗi câu hỏi con làm lộ rubric.
- Không đặt worked example cùng failure pattern ngay trước task.
- Không dựng stakeholder ngây ngô chỉ để phát biểu đúng lỗi vừa được dạy.
- Dữ liệu phải đủ, nhất quán và giống loại artifact có thể gặp trong thực tế.
- Nếu learner chưa làm đã được agent chỉ ra dữ kiện, phép kiểm tra và quyết định, task đang ở `GUIDED`.

## 5. Cold-read test

Trước khi coi module dùng được, đọc riêng phần đầu mà không dựa vào hội thoại. Nó phải cho phép một người mới trả lời:

- “Tôi sẽ nhận được kết quả gì?”
- “Trong tình huống nào tôi dùng cách này?”
- “Tôi cần làm hay nói câu nào tiếp theo?”
- “Tôi không cần làm điều gì?”

Nếu không trả lời được, viết lại bằng case thật; không thêm định nghĩa.

Cold-read test thất bại nếu người học phải đi qua state, rubric nội bộ hoặc biên bản chấm mới tìm thấy kiến thức và hành động chính.

## 6. Evals khi đóng gói skill

Đánh giá output trong context sạch, không chấm việc skill có nhiều file hay dùng đúng thuật ngữ. Tối thiểu có các case:

1. Người hoàn toàn mới chưa có schema.
2. Người đã có kinh nghiệm, cần bypass phần nhập môn.
3. Task rất ngắn, không cần framework.
4. Task dài có permission/cost/privacy checkpoint.
5. Người học nói “tôi không hiểu”.
6. Người học phản đối một kết luận/PASS cũ bằng bằng chứng mới.

Fatal failure: bắt learner dùng thuật ngữ nội bộ, dùng artifact như bằng chứng hiểu biết, hoặc tiếp tục bài mới sau tín hiệu không hiểu.
