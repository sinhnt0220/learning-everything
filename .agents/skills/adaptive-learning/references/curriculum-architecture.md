# Kiến trúc chương trình học

## 1. Định nghĩa đích đến

Không dùng “từ zero đến chuyên nghiệp” như một đích đủ rõ. Chuyển nó thành:

- **Output:** người học phải tạo ra, phân tích hoặc quyết định được gì?
- **Scope:** phần nào của lĩnh vực nằm trong khóa học và phần nào không?
- **Conditions:** phải thực hiện dưới ràng buộc nào về chất lượng, thời gian, an toàn hoặc công cụ?
- **Evidence:** sản phẩm hoặc hành vi nào chứng minh năng lực?

Nếu chưa có đủ context, đặt một giả định tạm thời. Chỉ hỏi một câu khi câu trả lời sẽ thay đổi đáng kể cấu trúc chương trình.

Sau đích đến, tạo **Domain Contract**: tiêu chuẩn đúng/sai, bằng chứng hợp lệ, source hierarchy, misconceptions, rủi ro, công cụ và external validation. Với sản phẩm/tool, tạo thêm Product Contract và surface/version snapshot.

## 2. Tầng phát triển

Các tầng này tổ chức curriculum, không phải trạng thái người dùng phải quản lý.

1. **Nền tảng:** ngôn ngữ, mô hình tinh thần và tiên quyết.
2. **Vận hành:** xử lý nhiệm vụ tiêu chuẩn có hỗ trợ.
3. **Độc lập:** xử lý biến thể, tự tìm lỗi và đọc nguồn.
4. **Chuyên nghiệp trong phạm vi:** tạo output thật dưới ràng buộc chất lượng.
5. **Chuyên sâu:** chọn một nhánh; không mở tất cả nhánh ngay từ đầu.

Không hứa hẹn “chuyên gia toàn ngành”.

## 3. Xương sống và nhánh

Với chủ đề rộng:

- Tạo một **xương sống** gồm các năng lực tiên quyết chung.
- Chỉ hiện các **nhánh** chuyên môn như lựa chọn tương lai.
- Chi tiết hóa 1–3 module kế tiếp; để các module sau ở mức outcome.
- Điều chỉnh bản đồ khi bằng chứng mới xuất hiện.

Không tạo curriculum dài chỉ để tạo cảm giác toàn diện.

## 4. Prerequisite graph

Mỗi năng lực cần biết:

- Cần năng lực nào trước?
- Nó mở khóa nhiệm vụ nào?
- Có thể học song song với gì?
- Cần công cụ hoặc môi trường nào?

Nếu người học thiếu tiên quyết, dạy đúng tiên quyết cần thiết thay vì mở một khóa phụ khổng lồ.

Mỗi node trong graph ghi target evidence stage. Quan hệ prerequisite chỉ được coi là thỏa khi stage thực tế đủ cho nhiệm vụ kế tiếp.

## 5. Ba cấp bằng chứng

### Module task

Kiểm tra một năng lực khóa và quyết định có thể đi tiếp hay cần sửa.

### Phase challenge

Kết hợp nhiều năng lực trong một tình huống ít hướng dẫn hơn. Dùng để phát hiện hiểu biết rời rạc.

### Capstone

Tạo artifact gần công việc thật, có yêu cầu không hoàn chỉnh, ràng buộc và tiêu chuẩn chất lượng. Capstone phải buộc người học tự đặt giả định, chọn công cụ, kiểm tra lỗi và giải thích quyết định.

## 6. Nhịp học và ma sát

- Mỗi lượt tương tác chỉ yêu cầu một hành động chính.
- Một module có thể kéo dài nhiều lượt nếu năng lực phức tạp.
- Không bắt mỗi lượt kết thúc bằng Proof Task; chỉ kiểm tra độc lập sau Readiness Gate.
- AI quản lý file, bằng chứng và next pointer.
- Người học không phải xác nhận roadmap hoặc chọn nhánh khi chưa có đủ context.
- Khi đã `PASS`, chuyển lớp mới. Không tiếp tục hỏi thêm chỉ để thấy chắc hơn.
- Dùng phase challenge và capstone để tăng độ tin cậy thay vì kéo dài từng module.

## 7. Tiêu chuẩn kết thúc

Khóa học chỉ kết thúc khi:

- Các năng lực xương sống trong phạm vi đã có bằng chứng.
- Phase challenge trọng yếu đã đạt.
- Capstone đạt rubric hoặc đã ghi rõ phần chưa đạt.
- Những năng lực chưa được kiểm chứng ngoài đời được liệt kê rõ.

Kết luận bằng “đã đạt phạm vi X”, không dùng danh xưng tuyệt đối.

## 8. Context packet

`learning-map.md` phải đủ để task mới tiếp tục mà không phụ thuộc trí nhớ hội thoại:

- Đích và phạm vi.
- Domain/Product Contract.
- Capability graph và evidence stage.
- Hiểu sai/bằng chứng mâu thuẫn đang mở.
- Source/version snapshot.
- Module hiện tại, artifact gần nhất và next pointer.
- Quyết định curriculum gần nhất.

Khi state mâu thuẫn artifact, ưu tiên artifact và ghi quyết định điều chỉnh.
