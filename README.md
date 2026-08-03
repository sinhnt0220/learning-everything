# Adaptive Learning

`adaptive-learning` là skill thiết kế và vận hành việc học dựa trên bằng chứng. Nó giúp một agent dạy theo loại năng lực và evidence thực tế, thay vì ép mọi chủ đề vào cùng một tutorial hoặc quiz.

## Skill làm gì?

- Thiết kế course, module và learning map cho khái niệm, lập trình, dữ liệu, khoa học thực nghiệm và phần mềm/AI tools.
- Dạy prerequisite trước khi yêu cầu người học tạo output; không coi thiếu kiến thức chưa dạy là lỗi của learner.
- Kiểm chứng artifact phù hợp với domain: code chạy được, execution log, file render, phép tính hoặc nguồn hiện hành.
- Tách bài học learner-facing khỏi learning map và evidence log nội bộ.
- Bảo vệ privacy, permission, chi phí và external side effects khi học công cụ.

## Cấu trúc

```text
.agents/skills/adaptive-learning/
├── SKILL.md
├── agents/openai.yaml
├── references/
└── templates/
```

`SKILL.md` là điểm vào. Các reference chỉ được đọc khi quyết định dạy cần chúng; templates dùng để tạo artifact khóa học.

## Dùng với Codex

Đặt folder `adaptive-learning` vào thư mục skills của workspace/runtime, rồi gọi:

```text
$adaptive-learning dạy tôi [chủ đề] theo trình độ hiện tại, có thực hành khi phù hợp.
```

Để học tiếp một course đã có, dùng `$adaptive-learning` và nói “học tiếp”. Skill sẽ đọc state nội bộ có liên quan trước khi chọn bài kế tiếp.

## Privacy boundary

Skill là phần có thể chia sẻ. Course cá nhân, learner profile, learning map và evidence log là dữ liệu riêng của người học; chúng không thuộc bản public release này.

## License

[MIT](LICENSE)
