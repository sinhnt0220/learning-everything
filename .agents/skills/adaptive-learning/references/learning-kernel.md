# Learning Kernel

## 1. Đơn vị thiết kế

Thiết kế theo **năng lực có thể quan sát**, không theo số trang hoặc danh sách thuật ngữ.

Mỗi module phải xác định:

- Người học sẽ làm được gì sau bài.
- Prerequisite nào cần có.
- Target evidence stage.
- Artifact/hành vi nào chứng minh đạt.
- Điều gì chỉ được mô phỏng và điều gì cần external validation.

Các thuộc tính trên là hợp đồng thiết kế nội bộ. Chúng phải có trong `learning-map.md` hoặc `work/evidence-log.md`, nhưng không phải trở thành các heading trong bài học learner-facing.

## 1.1. Hai lớp artifact

### Lớp learner-facing

`modules/*.md` chỉ chứa phần người học cần để hiểu hoặc thực hành:

- Kết quả thực tế và tình huống áp dụng.
- Kiến thức, ranh giới và cơ chế.
- Minh họa hoặc worked example khi support route thực sự cần.
- Ứng dụng, bài tập hoặc nguồn khi cần.

### Lớp vận hành nội bộ

- `learning-map.md`: state tổng hợp, prerequisite, capability graph, evidence stage và next pointer.
- `work/evidence-log.md`: bài nộp, mức hỗ trợ, cách kiểm chứng, kết quả chấm, giới hạn và điều kiện đổi đánh giá.

Readiness Gate, permission audit, rubric nội bộ và context handoff vẫn phải được chạy, nhưng không được dùng để kéo dài module learner-facing. Chỉ đưa một ranh giới quyền/an toàn vào bài học khi learner cần biết nó để thực hiện hành động hiện tại.

## 2. Chu trình dạy

Không dùng một chu trình hỗ trợ cố định. Chọn một trong ba support route:

```text
COLD: Định vị → Lý thuyết/cơ chế → Cold attempt → Feedback → Retry/Transfer

SCAFFOLDED: Định vị → Lý thuyết/cơ chế → Worked example/demo
→ Guided action → Independent Proof mới → Feedback

REMEDIATION: Lỗi đã quan sát → Giải thích một lỗi gốc
→ Retry sạch hoặc biến thể mới
```

Không bắt buộc hoàn thành cả chu trình trong một lượt. Một lượt chỉ cần một hành động nhận thức rõ.

Trước mọi task, chạy Task Gate trong `teacher-qa.md`. Block orientation được phép chỉ có case/trace và giải thích; “25 phút” không tự tạo nghĩa vụ phải có bài tập.

Support route mô tả hành vi dạy và đánh giá của Codex, không phải mục lục bắt buộc của một file module. Depth của kiến thức và lượng hỗ trợ là hai quyết định độc lập.

### Định vị

Nói khái niệm nằm ở đâu trong bức tranh lớn, giải quyết vấn đề gì và nối với năng lực trước nào. Không dùng context dài chỉ để tạo không khí.

### Khái niệm và cơ chế

- Định nghĩa từ mới trước khi dùng.
- Nêu ranh giới: nó là gì, không phải gì, dễ nhầm với gì.
- Giải thích quan hệ nhân quả/quy trình, input/output, điều kiện và giới hạn.
- Dùng ẩn dụ khi nó làm rõ; sau ẩn dụ phải quay lại cơ chế thật.
- Neo bài vào ít nhất một construct, cơ chế, phương pháp hoặc công cụ đặc hữu của domain. Kỹ năng chung như “tách fact khỏi inference” chỉ là phương tiện, không được thay thế nội dung môn học.

### Worked example/demo

- Không bắt buộc nếu prerequisite đã đủ, construct đơn giản và learner có thể cold attempt an toàn.
- Cho thấy toàn bộ đường đi từ input đến output.
- Làm lộ quyết định quan trọng và lý do, không chỉ kết quả.
- Với code/tool: chạy hoặc quan sát output thật.
- Với định lượng: hiện đơn vị, giả định và bước kiểm tra.
- Với case mở: chỉ rõ nhiều đáp án có thể hợp lý theo tiêu chí nào.
- Không dùng một worked example có cùng decision graph, failure pattern và output structure với task sẽ được chấm độc lập.

### Guided action

Chỉ dùng khi support route là `SCAFFOLDED` hoặc learner chủ động yêu cầu. Cho một biến thể gần, có gợi ý vừa đủ. Ghi mức hỗ trợ; kết quả tối đa ở stage `GUIDED`.

### Independent Proof

Chỉ giao sau Readiness Gate. Bối cảnh phải mới vừa đủ để tránh nhắc lại mẫu nhưng không đòi prerequisite chưa học. Brief nói rõ output và constraints nhưng không chia nhỏ đường suy luận thành checklist đáp án.

### Transfer

Sau vài module hoặc cuối phase, yêu cầu áp dụng trong boundary/context mới, tự chọn giả định/công cụ và bảo vệ quyết định.

## 3. Điều chỉnh theo nền

### Chưa có schema

Orientation ngắn → demo → mổ xẻ → guided action. Không dùng Socratic hoặc quiz thuật ngữ để “chẩn đoán”.

### Có nền nhưng chưa có evidence

Dùng cold challenge nhỏ hoặc artifact cũ để phân giải. Nếu đạt, khóa baseline; nếu không, chuyển sang remediation đúng prerequisite thiếu.

### Đã vận hành được

Dùng cold case biên, debugging, trade-off, phản ví dụ, transfer và nguồn gốc. Không làm lại tutorial nhập môn hoặc hướng dẫn phòng ngừa trước khi learner thử.

## 4. Tải nhận thức

- Một module có một năng lực khóa.
- Một orientation được phép nêu nhiều thành phần của bản đồ, nhưng hành động học chỉ tập trung vào một thành phần mới. Không giao bài phân loại nhiều thuật ngữ chỉ vừa được giới thiệu.
- Giới hạn thuật ngữ mới ở lượng cần thiết cho hành động hiện tại.
- Không giao đồng thời học khái niệm mới, chọn công cụ mới và xử lý dữ liệu thật nếu có thể tách.
- Dùng artifact nhỏ trước artifact thật khi môi trường có chi phí/rủi ro.
- Một hành động chính có thể chứa nhiều bước tự nhiên bên trong; không biến nó thành hàng loạt câu hỏi vụn.

## 4.1. Nhịp block và lab thao tác

Mặc định thiết kế một module learner-facing cho khoảng **25 phút** làm việc thực: định vị/đọc ngắn → hiểu cơ chế → thực hành hoặc phân tích khi Task Gate đạt → kiểm tra/feedback khi cần.

- Với tool, Git, automation hoặc product, gom nhiều click/câu lệnh vào một lab khi chúng cùng tạo một outcome, artifact và permission boundary.
- Không tạo module chỉ để chuyển một state UI, chụp màn hình hoặc xác nhận một click đã xảy ra.
- Tách lab khi learner phải dùng năng lực mới, đối mặt side effect/permission mới, hoặc cần một điểm proof độc lập.
- `MICRO` có thể là một tương tác chat ngắn, không cần file. `DEEP` có thể qua nhiều block; không ép hoàn thành trong 25 phút.
- Cập nhật learning map/evidence log sau một lab/phase; riêng commit, push, merge, publish hoặc chi phí phải được ghi ngay sau khi xảy ra.

## 5. Retrieval và tích lũy

- Cài kiến thức cũ vào bài mới thay vì tạo lịch ôn bắt buộc.
- Khi kiến thức cũ thất bại trong bối cảnh mới, mở remediation ngắn rồi quay lại dòng chính.
- Module chứng minh một năng lực; phase challenge chứng minh phối hợp; capstone chứng minh performance gần thực tế.

## 6. Tinh hoa từ Fei Fei cũ

Giữ khi phù hợp:

- Context & Anatomy.
- Mechanism.
- Cognitive Bridge.
- Case gần đời thật.
- Giải thích rồi vận dụng.
- Feedback chỉ ra Aha Moment có bằng chứng.

Không ép:

- First Principles cho mọi bài.
- Feynman cho mọi domain.
- Ẩn dụ vật lý/sinh học/tiến hóa không có cơ sở.
- Cá nhân hóa thành chẩn đoán tâm lý.
- Giọng khoa trương hoặc danh hiệu thay cho rubric.
