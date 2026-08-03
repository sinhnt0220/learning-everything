# Đánh giá và bằng chứng năng lực

## 1. Tách stage khỏi kết quả

### Evidence stage

| Stage | Ý nghĩa | Bằng chứng điển hình |
|---|---|---|
| `UNVERIFIED` | Chưa có bằng chứng | Chỉ có self-report hoặc chưa học |
| `INTRODUCED` | Đã được giới thiệu | Đã đọc/nghe orientation |
| `MODELED` | Đã quan sát ví dụ hoàn chỉnh | Nhận diện được input, bước và output |
| `GUIDED` | Làm được với checklist/gợi ý | Artifact có trợ giúp đáng kể |
| `INDEPENDENT` | Làm biến thể gần không cần gợi ý quyết định | Artifact chạy/đúng và giải thích được |
| `TRANSFER` | Dùng trong context mới, tự chọn giả định/công cụ | Phase challenge/case mới |
| `EXTERNAL_VALIDATION` | Được môi trường ngoài AI xác nhận | Lab, production, stakeholder, user, peer review |

### Kết quả một lần chấm

- `PASS`: đạt target stage đã công bố.
- `REVISE`: có một lỗi gốc cần sửa trước khi đạt target stage.
- `CHƯA ĐỦ BẰNG CHỨNG`: thiếu artifact, khả năng quan sát hoặc chuẩn đủ chắc.
- `TEACHING GAP`: thiết kế task thiếu prerequisite, nguồn hoặc tiêu chí đã dạy. Đây là lỗi curriculum, không phải kết quả của learner; hủy chấm và sửa/dạy lại.

Luôn ghi `PASS ở stage nào`; không dùng PASS trần như chứng nhận toàn khóa.

## 2. Quy tắc chuyển stage

- “Tôi hiểu”, lời giải thích trôi chảy hoặc Permanent Note không tự tăng stage.
- Sau khi xem demo: tối đa `MODELED`.
- Làm lại từng bước theo hướng dẫn: tối đa `GUIDED`.
- `INDEPENDENT` cần biến thể/requirement mới, artifact được kiểm chứng và không có gợi ý quyết định.
- `TRANSFER` cần context/boundary mới và tự chọn giả định/công cụ.
- `EXTERNAL_VALIDATION` không được tự cấp trong chat.
- Bằng chứng mâu thuẫn được phép hạ stage; ghi lý do và mở remediation ngắn.

## 3. Proof Task hợp lệ

Một Independent Proof phải:

- Chỉ xuất hiện sau Readiness Gate.
- Đo đúng một năng lực khóa và target stage.
- Dùng biến thể mới nhưng không nhảy prerequisite.
- Không lộ đáp án hoặc decision path trong hướng dẫn/example.
- Công bố output, constraints và chuẩn chất lượng. Không công bố checklist chi tiết nếu các mục đó chính là những suy luận learner phải tự tạo.
- Có cách kiểm chứng bằng nguồn, tool hoặc artifact.
- Ghi mức hỗ trợ đã dùng.

Không mặc định Feynman. Giải thích không thay thế chạy code, tính toán, execution, data analysis, protocol, revision hoặc decision.

### Anti-priming và mức hỗ trợ

- Theory về construct không tự làm mất tính độc lập.
- Worked example có cấu trúc khác task có thể là `MODELED`, nhưng phải kiểm tra transfer.
- Example/checklist/câu hỏi con cùng decision graph với task làm evidence tối đa `GUIDED`.
- Feedback sau cold attempt là remediation. Retry chỉ được coi là `INDEPENDENT` khi đáp án chưa bị lộ hoặc dùng một biến thể sạch.
- Không trừ điểm learner vì đề thiếu dữ kiện, tự mâu thuẫn hoặc stakeholder bị dựng phi thực tế; sửa assessment trước.
- Không chấm việc learner tự suy diễn license, documentation, bug hay contribution scope nếu cách đọc/kiểm chứng chúng chưa được dạy như năng lực của module.

## 4. Rubric

Chọn các trục liên quan:

- **Đúng:** output/kết luận có đúng không?
- **Cơ chế:** có hiểu vì sao và data/process đi thế nào không?
- **Artifact:** có tồn tại, chạy/render/tính lại được không?
- **Chuyển giao:** có xử lý biến thể/context mới không?
- **Độc lập:** cần bao nhiêu gợi ý?
- **Kiểm chứng:** có test, log, nguồn, đơn vị hoặc assumptions không?
- **Giới hạn:** có biết điều gì chưa kết luận được không?
- **An toàn/quyền:** có tuân thủ permission, privacy, consent và chi phí không?

## 5. Kiểm chứng theo domain

- Code: chạy, test, edge case và đọc lỗi.
- Automation: test input, execution log, dữ liệu trung gian, output và retry/error path.
- AI media: file render, brief, so sánh phiên bản, revision và quyền asset/voice.
- Số liệu: tính lại, đơn vị, denominator, assumptions và sensitivity.
- Data Science: data quality, leakage, split, metric, reproducibility và overclaim.
- Khoa học/thực nghiệm: cơ chế, điều kiện, protocol, sai số, nguồn và an toàn; không công nhận lab từ mô phỏng.
- Xã hội/tâm lý/lịch sử: tách observation, construct, inference, fact và value judgment; nguồn cạnh tranh, boundary và ethics.
- Hệ thống: boundary, biến số, polarity, feedback, delay, assumptions, counterexample và intervention.
- Sáng tạo: brief, kỹ thuật, hiệu quả artifact và revision; không giả vờ có một đáp án thẩm mỹ duy nhất.

## 6. Phản hồi

### PASS

1. Nêu target stage và artifact cụ thể.
2. Nêu tiêu chí đã đạt.
3. Nêu giới hạn/external validation.
4. Cập nhật map và chuyển lớp.

### REVISE

1. Nêu lỗi gốc trước.
2. Giải thích cơ chế sai.
3. Giao một sửa đổi ngắn; không giao lại toàn bài.

### CHƯA ĐỦ BẰNG CHỨNG

Nói thiếu gì và yêu cầu đúng một artifact/dữ kiện có sức phân giải cao.

### TEACHING GAP

Nói rõ task đã đòi điều gì chưa được dạy, hủy yêu cầu retry và quay về orientation/demo. Ghi lỗi ở curriculum, không ở learner.

## 7. Rolling diagnosis và retention

Theo dõi:

- Đã chứng minh và stage.
- Chưa chứng minh.
- Hiểu sai/bằng chứng mâu thuẫn.
- Điều kiện đổi đánh giá.

Cài retrieval tự nhiên vào bài mới. Dùng phase challenge/capstone để kiểm tra phối hợp và transfer; không kéo dài một module bằng quiz cùng cấp.

## 8. Lưu evidence và state

Không dùng module learner-facing làm hồ sơ chấm.

- Ghi từng lần nộp/chấm vào `work/evidence-log.md`: ngày, module/capability, artifact hoặc câu trả lời, mức hỗ trợ, cách kiểm chứng, kết quả, stage trước/sau, giới hạn và next action.
- `learning-map.md` chỉ giữ evidence ledger tóm tắt, chẩn đoán làm việc và next pointer; link tới entry chi tiết khi cần.
- Không sao chép nguyên văn cùng một bằng chứng vào cả module, learning map và evidence log.
- Không sửa nội dung kiến thức của module chỉ để phản ánh một lần PASS/REVISE. Nếu feedback làm lộ lỗi kiến thức trong bài, sửa bài như một content revision riêng và ghi quyết định trong map/log.
- Nếu khóa học cũ chưa có `work/evidence-log.md`, đọc evidence lịch sử ở module/map nhưng ghi các lần đánh giá mới vào evidence log; không bắt buộc migrate toàn bộ lịch sử ngay.
