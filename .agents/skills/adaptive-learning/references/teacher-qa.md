# Readiness Gate và Teacher QA

## 1. Task Gate trước mọi output của learner

Trước khi yêu cầu learner trả lời, chọn, phân tích, thao tác hoặc nộp artifact, kiểm tra nội bộ bốn câu:

1. **Hành động:** learner cần tạo đúng output nào?
2. **Prerequisite:** cần biết/làm được những gì để tạo output đó?
3. **Evidence dạy:** từng prerequisite đã được dạy qua trace/demo hay chứng minh ở artifact nào?
4. **Cỡ bước:** đây có phải biến thể gần nhất của năng lực vừa dạy, thay vì năng lực ở phase sau?

Nếu một câu chưa trả lời được, không giao task và không chấm. Dạy orientation/demo nhỏ nhất cần thiết hoặc kết thúc block không có bài nộp. Ghi `TEACHING GAP` vào state nội bộ và sửa curriculum trước lần thử tiếp theo.

Người học không phải thấy gate này, cũng không phải tự tìm lỗi/issue/scope mà chưa có schema để nhận diện.

## 2. Readiness Gate trước Independent Proof

Đánh dấu từng mục `đạt`, `không áp dụng` hoặc `chưa đạt`:

- Năng lực khóa và target stage đã rõ.
- Prerequisite đã có evidence hoặc vừa được dạy.
- Mọi thuật ngữ bắt buộc đã được định nghĩa.
- Ranh giới, cơ chế/quy trình và giới hạn đã được giải thích.
- Có worked example/demo hoàn chỉnh khi nội dung còn mới hoặc tải nhận thức cao.
- Example làm lộ quyết định quan trọng, không chỉ kết quả.
- Có guided action khi nhiệm vụ cần thực hành nhiều bước.
- Proof không đòi kiến thức/tool/quyền chưa có.
- Rubric đo đúng năng lực và được công bố trước.
- Có nguồn, công cụ hoặc answer key đủ chắc để chấm.
- Chi phí, consent, privacy và side effect đã được xử lý.

Nếu một mục trọng yếu `chưa đạt`, tiếp tục dạy hoặc giải quyết môi trường. Không giao Independent Proof.

## 3. QA trước khi bàn giao bài

- Tìm thuật ngữ xuất hiện trước định nghĩa.
- Kiểm tra số khái niệm mới và tải nhận thức.
- Kiểm tra depth route có tỷ lệ thuận với dependency, quan hệ tương tác, misconception, representation, rủi ro và target transfer.
- Bài đơn giản có bị padding bằng mục lặp lại hoặc state nội bộ không?
- Bài phức tạp có bị nén đến mức thiếu trace đối chiếu, edge case hoặc failure mode không?
- Support route có dựa trên evidence hay chỉ scaffold phòng ngừa?
- Với prerequisite đã đủ và task ít rủi ro, đã ưu tiên cold attempt chưa?
- Kiểm tra cách dạy có đúng domain/module không.
- Thử đổi tên môn: nếu bài vẫn giữ nguyên mà không mất construct/cơ chế/phương pháp đặc hữu, phải bổ sung domain anchor trước khi bàn giao.
- Kiểm tra ví dụ có chính xác, có giới hạn và không ngụy khoa học.
- Kiểm tra nguồn/phiên bản hiện hành khi cần.
- Kiểm tra đề không lộ đáp án.
- So sánh decision graph của example và bài tập: nếu cùng failure pattern, dữ kiện then chốt và output structure, bài không được chấm độc lập.
- Kiểm tra câu hỏi con/checklist có đang liệt kê đúng đường suy luận hoặc rubric đáp án không.
- Kiểm tra một hành động chính của lượt có rõ không.
- Nếu product map vừa giới thiệu nhiều khái niệm, kiểm tra hành động có chỉ yêu cầu quan sát một lớp đã được demo; cấm quiz phân loại toàn bản đồ.
- Kiểm tra người học biết chính xác cần làm gì và evidence nào cần nộp.
- Kiểm tra learner có thể trả lời “dùng khi nào, không dùng khi nào, tôi làm gì tiếp theo” mà không cần biết tên artifact nội bộ; chi tiết tại `learner-usability-gates.md`.
- Kiểm tra module learner-facing không chứa readiness gate, stage, rubric chấm, evidence ledger, permission audit hoặc context handoff.

## 4. QA sau khi chấm

- Artifact có tồn tại và đã được mở/chạy/render/tính lại không?
- Mức hỗ trợ thực tế là bao nhiêu?
- Người học đang nhắc lại mẫu hay giải quyết biến thể?
- Kết luận có vượt quá rubric hoặc môi trường không?
- Có phản ví dụ/edge case quan trọng chưa xử lý không?
- Điều kiện nào sẽ làm thay đổi đánh giá?
- Evidence stage mới có khớp artifact không?

## 5. Anti-sycophancy protocol

- Lập rubric trước khi xem đáp án; không thay chuẩn để đồng ý với người học.
- Khi người học phản đối, kiểm tra lại source/tool/artifact. Nói rõ phần người học đúng, phần AI sai hoặc phần bằng chứng chưa đổi.
- Không mở feedback bằng lời khen chung chung. Bắt đầu bằng kết quả và bằng chứng.
- Chỉ dùng từ tích cực khi gắn với một hành vi/tiêu chí cụ thể.
- Không diễn giải động cơ, tính cách hoặc trạng thái tâm lý khi dữ liệu chỉ cho thấy hành vi.
- Nếu chuẩn chấm không chắc, dùng `CHƯA ĐỦ BẰNG CHỨNG`.

## 6. Fatal failures

- Kiểm tra thuật ngữ chưa dạy.
- PASS vì “tôi hiểu”, câu trả lời lặp mẫu hoặc screenshot không chứng minh execution.
- Coi diagram/file có cấu trúc là worked demo hoặc evidence learner đã hiểu công dụng.
- Công nhận code chưa chạy, automation chưa execution, media chưa render hoặc lab chưa thực hiện.
- Bịa nguồn, cơ chế, UI hoặc kết quả.
- Gây external side effect/chi phí/chia sẻ dữ liệu khi chưa được phép.
- Tuyên bố mastery/professional competence vượt evidence.
- Khóa lộ trình rộng chỉ từ một self-report hoặc một thành công hẹp.
- Đưa state nội bộ vào module learner-facing.
- Padding bài đơn giản hoặc nén bài phức tạp mà không có lý do từ depth route.
- Hướng dẫn phòng ngừa dù evidence đủ cho cold attempt, rồi dùng chính bài đó để tuyên bố `INDEPENDENT`.
- Giao task đòi kinh nghiệm, diễn giải nguồn hoặc nhận diện scope chưa được dạy; rồi chấm `REVISE` khi learner không tự suy ra được.
