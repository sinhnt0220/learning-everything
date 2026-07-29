# Kỷ luật nguồn và độ chắc chắn

## 1. Phân loại tài liệu người học đưa

Trước khi sử dụng, xác định tài liệu là:

1. Nguồn nội dung cần học.
2. Mẫu cấu trúc hoặc cách trình bày.
3. Ẩn dụ về trải nghiệm học.
4. Bài làm hoặc bằng chứng năng lực của người học.

Không trộn nội dung của mẫu cấu trúc vào môn mới. Nếu vai trò chưa rõ và làm thay đổi kết quả, hỏi một câu; nếu không, nêu giả định ngắn.

## 2. Xương sống nguồn

Mỗi khóa học rộng cần một nhóm nguồn lõi vừa đủ:

- Nguồn chính thức hoặc tiêu chuẩn đối với công cụ và kỹ thuật thay đổi nhanh.
- Giáo trình chuẩn, paper gốc hoặc tổ chức chuyên môn đối với khoa học.
- Tác giả/công trình nền tảng cùng các phê bình đáng tin đối với trường phái lý thuyết.
- Dataset, code và protocol có thể tái lập đối với môn thực hành.
- Help center, release notes, pricing/plan và UI hiện hành đối với product/tool thay đổi nhanh.

Không biến danh sách nguồn thành một thư viện khổng lồ. Gắn nguồn với phase hoặc quyết định mà nó hỗ trợ.

## 3. Khi phải nghiên cứu lại

Kiểm tra nguồn hiện hành khi:

- Phiên bản phần mềm, API, tiêu chuẩn hoặc best practice có thể đã đổi.
- Chủ đề có rủi ro an toàn, sức khỏe, pháp lý hoặc tài chính.
- Người dùng yêu cầu nguồn, trích dẫn hoặc độ chính xác cao.
- AI không chắc về một fact, công thức, lịch sử hoặc thuật ngữ chuyên ngành.
- Giao diện, feature, plan, credit, quyền sử dụng hoặc giới hạn vùng có thể đã đổi.

Ưu tiên nguồn chính thức và nguồn gốc. Phân biệt rõ fact, suy luận và khuyến nghị.

Với product/tool, lưu ngày kiểm tra và surface/version snapshot; dạy theo mục tiêu semantic thay vì chỉ vị trí nút. Khi UI khác tài liệu, quan sát state hiện tại và refresh nguồn, không bịa thao tác.

## 4. Quy tắc giải thích

- Không ép mọi khái niệm phải được lý giải bằng vật lý, tiến hóa, sinh học hoặc triết học.
- Dùng First Principles khi có cấu trúc nhân quả thật sự và giúp giải quyết nhiệm vụ.
- Dùng ẩn dụ như cầu nối, không như bằng chứng.
- Nêu điều kiện áp dụng và phản ví dụ quan trọng.
- Không khẳng định “ghim vĩnh viễn”, “chắc chắn” hoặc “đúng tuyệt đối” khi không có cơ sở.

## 5. Quy tắc chấm

AI không được dùng sự tự tin của chính mình làm chuẩn đáp án.

- Với bài có đáp án xác định, lập answer key hoặc rubric từ nguồn/công cụ trước khi chấm.
- Với bài mở, nêu các trục đánh giá và chấp nhận nhiều lời giải hợp lý.
- Khi nguồn mâu thuẫn, trình bày tranh luận và tiêu chuẩn lựa chọn.
- Nếu chưa kiểm chứng được, dùng `CHƯA ĐỦ BẰNG CHỨNG` thay vì ép PASS/REVISE.

Nguồn do vendor viết có thể đủ để xác nhận thao tác/feature nhưng không tự đủ để xác nhận hiệu quả học tập, chất lượng sáng tạo hoặc claim marketing. Tách tài liệu vận hành khỏi bằng chứng hiệu quả.

## 6. Ghi nguồn trong course

- `learning-map.md` lưu source backbone.
- Module chỉ ghi nguồn trực tiếp hỗ trợ nội dung hoặc rubric của module.
- `exports/` giữ các nguồn quan trọng đủ để người học kiểm tra lại sau này.
