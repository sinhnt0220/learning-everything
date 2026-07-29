# Bộ định tuyến độ sâu bài học

Độ dài không đồng nghĩa với độ sâu. Chọn độ sâu theo cấu trúc kiến thức và mức chuyển giao cần đạt, không theo số chữ cố định hoặc quy tắc mọi module phải truyền tải lượng kiến thức như nhau.

## 1. Sáu tín hiệu định tuyến

Đánh giá trước khi soạn bài:

- số prerequisite mới;
- số quan hệ hoặc bước tương tác;
- misconception và edge case quan trọng;
- số representation learner phải nối với nhau;
- hậu quả nếu hiểu sai;
- độ phức tạp của tình huống transfer đích.

“Một module, một năng lực khóa” kiểm soát phạm vi. Nó không buộc mọi năng lực phải được dạy trong cùng một dung lượng.

## 2. Ba chế độ độ sâu

### MICRO

Dùng khi chỉ có một distinction, rule hoặc thao tác cục bộ, ít phụ thuộc và rủi ro thấp.

- Ưu tiên trả lời ngay trong chat.
- Dạy kết quả, rule/cơ chế ngắn và một ví dụ sát.
- Không tạo file nếu không có nhu cầu lưu bền.
- Không padding bằng roadmap, rubric, state hoặc các mục lặp lại.

### STANDARD

Dùng khi learner cần hiểu một cơ chế hoàn chỉnh và áp dụng trong biến thể gần.

- Định nghĩa và ranh giới.
- Cơ chế hoặc quy trình.
- Một minh họa ngắn hoặc worked example chỉ khi support route cần; không bắt buộc.
- Một boundary, counterexample hoặc lỗi thường gặp có ý nghĩa.
- Một ứng dụng để learner tự xử lý.

### DEEP

Dùng khi nhiều construct/bước tương tác, sai lầm có hậu quả, hoặc target đòi transfer xa.

- Làm rõ prerequisite và quan hệ giữa chúng.
- Dùng ít nhất hai trace, case đối chiếu hoặc representation bổ sung nhau.
- Dạy failure modes, edge cases và điều kiện đổi kết luận.
- Có thể kéo dài nhiều lượt hoặc tách thành nhiều module.
- Không nén một năng lực phức tạp vào cùng dung lượng với bài đơn giản.

## 3. Khi nào phải tách module

Tách khi:

- có hơn ba dependency mới mà learner phải giữ đồng thời;
- learner phải học construct mới, tool mới và dữ liệu thực cùng lúc;
- một phần có thể đạt target stage độc lập trước phần còn lại;
- worked example cần nhiều quyết định chưa được dạy;
- nội dung đang biến thành danh sách khái niệm thay vì một cơ chế có thể dùng.

Tách theo capability hoặc dependency, không cắt cơ học theo số chữ.

## 4. Quy tắc chống đồng phục

- Không dùng word count hoặc tỷ lệ phần trăm nội dung làm KPI chất lượng.
- Bài đơn giản phải ngắn; không thêm mục chỉ vì template có chỗ trống.
- Bài phức tạp được phép dài hoặc nhiều lượt nếu mỗi phần phục vụ năng lực khóa.
- Template là khung tối thiểu, không phải checklist buộc điền mọi mục.
- Nếu learner đã có evidence mạnh, có thể bỏ phần cơ bản và chuyển thẳng sang counterexample, debugging hoặc transfer challenge.

## 5. Support route độc lập với depth

Độ sâu trả lời “kiến thức phức tạp đến đâu”. Support route trả lời “learner cần được hỗ trợ trước khi thử đến mức nào”. Không suy từ `STANDARD/DEEP` rằng luôn phải có worked example.

## 5.1. Gom thao tác thành lab

Số click, screenshot hay command không quyết định số module. Với product/tool, gom chúng vào cùng một lab khi learner đang tạo một outcome hoặc artifact duy nhất dưới cùng permission boundary.

Tách lab khi có một trong các điều kiện sau:

- learner phải vận dụng một capability mới;
- xuất hiện tool, dữ liệu, quyền hoặc side effect mới;
- cần proof độc lập thay vì chỉ xác nhận state;
- tải nhận thức vượt block mặc định khoảng 25 phút.

Ví dụ: tạo branch → stage scope → commit → push → mở draft PR là một release lab có checkpoints an toàn; không phải năm module chỉ vì có năm thao tác.

### `COLD`

Dùng mặc định khi prerequisite đã đủ, task có thể đảo ngược/ít rủi ro và learner đã có reasoning nền liên quan.

- Dạy theory/reference cần thiết.
- Giao một output thực tế duy nhất.
- Không chia thành câu hỏi con tương ứng với rubric.
- Không cho worked example có cùng cấu trúc suy luận.

### `SCAFFOLDED`

Dùng khi learner chưa có schema, thao tác có nhiều bước phụ thuộc, tải nhận thức cao hoặc sai sót có rủi ro.

- Worked example/demo trước.
- Guided action gần.
- Muốn chấm `INDEPENDENT` phải dùng task mới không trùng decision path.

### `REMEDIATION`

Dùng sau khi đã quan sát một lỗi hoặc misunderstanding.

- Chỉ giải thích lỗi gốc và cơ chế liên quan.
- Không làm hộ toàn bài.
- Giao retry sạch; nếu retry dùng lại task đã lộ đáp án, stage tối đa là `GUIDED`.

## 6. Anti-priming

Trước khi giao bài, so sánh teaching artifact và assessment:

- Chúng có cùng failure pattern không?
- Các câu hỏi con có liệt kê đúng các bước cần suy ra không?
- Example có chỉ sẵn dữ kiện quan trọng và quyết định cần đưa ra không?
- Learner chỉ cần thay số hoặc đổi danh từ để trả lời không?

Nếu có, task đang được guided. Hoặc thay task, hoặc chấm đúng stage `GUIDED`.

## 7. Output nội bộ

Trước khi dạy, Codex ghi ngắn trong learning map hoặc context packet:

- depth route: `MICRO | STANDARD | DEEP`;
- support route: `COLD | SCAFFOLDED | REMEDIATION`;
- tín hiệu chính dẫn đến route;
- module có cần tách hay không;
- representation/example bắt buộc.

Không đưa phân loại depth hoặc lý do điều phối vào module learner-facing trừ khi learner hỏi về thiết kế khóa học.
