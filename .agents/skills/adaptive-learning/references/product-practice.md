# Practice-first Product Learning

Áp dụng cho automation, AI video/music, design tools, SaaS và phần mềm thay đổi nhanh.

## 1. Product Contract

Trước bài đầu, ghi:

- Outcome/artifact cần tạo.
- Product surfaces và mental model tối thiểu.
- Tài khoản, plan, thiết bị và quyền truy cập.
- Credits/chi phí/paywall liên quan.
- Dữ liệu được đưa lên dịch vụ.
- Side effects có thể xảy ra.
- Nguồn chính thức và ngày kiểm tra.
- Bằng chứng thực hành có thể quan sát.

Nếu người học chưa biết gì, không hỏi họ định nghĩa thuật ngữ. Chọn một artifact nhỏ, riêng tư, đảo ngược được và dùng mock data/draft/manual mode.

## 2. Product map trước khi click

Giải thích đủ dùng:

- Công cụ giải quyết vấn đề gì.
- Surface chính đang dùng.
- `Input → xử lý → output`.
- Đối tượng cốt lõi trong giao diện.
- Dấu hiệu chạy thành công/thất bại.
- Draft/test khác activate/publish/send ở đâu.

Không kiểm tra product map như bài thuộc lòng.

Nếu map có nhiều lớp/khái niệm mới:

1. Giới thiệu map để định vị, không dùng làm Proof Task.
2. Chọn một lớp có artifact thật gần nhất với kinh nghiệm hiện có.
3. Cho xem cấu trúc, input/output và trace khi lớp đó được kích hoạt.
4. Cho một guided observation/modification của đúng lớp đó.
5. Chỉ so sánh/phân loại nhiều lớp sau khi từng lớp cần thiết đã đạt ít nhất `MODELED`.

## 3. Practice ladder

| Mức | Người học làm gì | Evidence tối đa |
|---|---|---|
| `OBSERVE` | Xem demo với input, bước, output và tín hiệu thành công | `MODELED` |
| `REPRODUCE` | Làm lại với checklist/gợi ý | `GUIDED` |
| `EXPLAIN` | Chỉ ra vai trò thành phần, data flow và tham số | `GUIDED` |
| `MODIFY` | Thay input/điều kiện/style/cấu trúc/node/scene/section | `INDEPENDENT` nếu không cần gợi ý quyết định |
| `DEBUG` | Đọc lỗi, tìm bước hỏng, kiểm tra trung gian, sửa và chạy lại | `INDEPENDENT` |
| `BUILD` | Tự tạo artifact gần nhu cầu thật | `INDEPENDENT` hoặc `TRANSFER` theo độ mới |
| `OPERATE` | Chạy lại, theo dõi, version, chi phí, quyền và khi không nên dùng | `TRANSFER`; production cần external validation |

Không buộc mọi module đi qua cả bảy mức. Toàn phase phải có progression từ quan sát đến vận hành.

## 4. Automation adapter

Mental model:

```text
Trigger → Input data → Transformation/logic → Action → Output
→ Execution history/error
```

Thứ tự ưu tiên:

1. Orientation: workflow/scenario, node/module, connection, execution.
2. Chạy template/workflow mẫu bằng mock data.
3. Quan sát dữ liệu ở từng bước.
4. Thay/thêm node hoặc module.
5. Dạy mapping, filter và branch trên dữ liệu nhìn thấy được.
6. Tạo lỗi an toàn và đọc execution log.
7. Test manual trước schedule/activate.
8. Xây workflow thật.
9. Chỉ thêm error handling, idempotency, secrets và cost monitoring khi scope cần.

PASS vận hành cần execution evidence, output đúng, giải thích data flow và ít nhất một modification/debug. Import template, ảnh canvas hoặc một run không hiểu data flow chưa đủ.

## 5. AI video adapter

Mental model:

```text
Mục tiêu/audience/format → Script → Scene/shot → Avatar/voice/visual
→ Generate/render → Review → Edit → Export
```

- Bắt đầu bằng draft riêng tư 20–30 giây.
- Thay script/scene rồi so sánh hai phiên bản theo rubric.
- Review pacing, phát âm, caption, visual và consistency.
- Chỉ dùng digital twin/voice cloning/API sau consent, privacy và cost orientation.

PASS cần video render thật, ít nhất một revision có lý do, khả năng truy nguyên lỗi/chất lượng về thành phần và quyền hợp lệ với asset/voice/avatar.

## 6. AI music/audio adapter

Mental model:

```text
Ý đồ → Lyrics/instrumental → Style/cấu trúc → Generation
→ So sánh → Section editing/arrangement → Export/quyền
```

- Bắt đầu ở chế độ đơn giản để thấy input/output.
- So sánh biến thể bằng brief, cấu trúc, nhất quán và khả năng sử dụng.
- Chuyển sang custom/advanced khi người học đã hiểu thành phần điều khiển.
- Yêu cầu sửa style, lyrics hoặc section; generation đầu chưa chứng minh vận hành.

## 7. Quyền, chi phí và side effects

Hard stop:

- Không yêu cầu password, token hoặc API key trong chat.
- Không dùng dữ liệu khách hàng thật ở bài đầu.
- Không activate, schedule, publish, send hoặc share externally khi chưa được phép.
- Không tiêu credits có phí khi chưa thông báo và được đồng ý.
- Không upload khuôn mặt/giọng nói/dữ liệu cá nhân của người khác khi chưa có consent.
- Không vượt paywall để “hoàn thành bài”; đưa lựa chọn free/mock/alternative.

Nếu Codex không quan sát được giao diện, dùng screenshot, export, execution log hoặc file render. Không có bằng chứng chạy/render thì stage tối đa là `MODELED`.

## 8. Chống UI drift

- Kiểm tra help center/docs/release notes chính thức tại ngày bắt đầu khóa và trước module dùng feature dễ đổi.
- Lưu surface/version snapshot trong learning map.
- Dạy theo mục tiêu semantic, không phụ thuộc duy nhất vào vị trí nút.
- Khi UI khác tài liệu, dừng, quan sát state hiện tại và refresh nguồn; không bịa thao tác.

## 9. Extension architecture adapter

Áp dụng khi học Plugin, Skill, App, MCP, Config, Hook hoặc các lớp mở rộng tương tự.

- Product map được phép nêu quan hệ toàn cảnh nhưng không phải bài kiểm tra.
- Module đầu chọn một artifact đang có thật, ví dụ một Skill folder, plugin manifest, MCP tool listing, config entry hoặc hook trace.
- Dạy theo chuỗi `artifact nằm ở đâu → hệ thống đọc/kích hoạt thế nào → input/output → dấu hiệu quan sát → giới hạn/lỗi`.
- Guided action là quan sát hoặc thay đổi an toàn trên artifact đó, không phải ghép tên với định nghĩa.
- Chỉ mở lớp tiếp theo khi lớp hiện tại đạt `MODELED` hoặc target stage đã định.
- Bài so sánh kiến trúc chỉ hợp lệ sau khi các lớp được so sánh đều đã có concrete example.
