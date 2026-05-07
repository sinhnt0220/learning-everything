---
name: novel-writer-workflow-guide
description: "Sử dụng khi người dùng bắt đầu một dự án tiểu thuyết hoặc hỏi cách tổ chức việc viết lách của họ - hướng dẫn qua phương pháp luận 7 bước của một tác giả và đảm bảo quy trình làm việc chuẩn xác"
allowed-tools: Read, Grep
---

# Hướng Dẫn Quy Trình Viết Tiểu Thuyết Bằng Hệ Thống (Novel Writer Workflow)

## Khi người dùng nói "Tôi muốn viết tiểu thuyết"

**Kích hoạt ngay hướng dẫn luồng công việc này.**

## Tổng quan Phương pháp luận 7 bước

```
1. /constitution  → Thiết lập Nguyên tắc sáng tác (Hiến pháp truyện)
2. /specify       → Định nghĩa Đặc tả câu chuyện (Bối cảnh, mạch truyện)
3. /clarify       → Làm rõ các điểm mù / Mâu thuẫn
4. /plan          → Lên kế hoạch chi tiết (Dàn ý, Cấu trúc)
5. /tasks         → Phân rã thành các Task công việc 
6. /write         → Tiến hành Viết
7. /analyze       → Kiểm định chất lượng và sự nhất quán
```

## Hướng dẫn Chi tiết từng Bước

### Bước 1: Thiết lập Nguyên tắc sáng tác (Hiến pháp truyện)

> "Hãy bắt đầu bằng lệnh `/constitution` để định nghĩa rõ Nguyên tắc sáng tác của bạn. Bước này sẽ thiết lập các giá trị cốt lõi, tiêu chuẩn chất lượng và những luật lệ bất di bất dịch của câu chuyện (Ví dụ: AI không được viết thay, Tác giả là người chắp bút)."

**Tại sao bước này quan trọng**: Đóng vai trò là "Bản Hiến Pháp Sáng Tác" của bạn - mọi quyết định về sau đều phải đối chiếu với các nguyên tắc này.

**Bao gồm những gì**:
- Giá trị cốt lõi (Thông điệp hoặc tư tưởng muốn truyền tải)
- Giới hạn chất lượng (Vùng cấm tuyệt đối không thỏa hiệp)
- Nguyên tắc văn phong (Ví dụ: Tảng băng trôi, nhịp độ dồn dập, kiệm lời)
- Nguyên tắc nội dung (Quy luật xây dựng nhân vật, cốt truyện, thế giới quan)

**Thời gian dự kiến**: 15-20 phút

### Bước 2: Định nghĩa Đặc tả câu chuyện

> "Bây giờ hãy sử dụng `/specify` để tạo ra một Bản đặc tả câu chuyện giống hệt như thiết kế một Sản phẩm (Product Spec). Hãy tư duy như một Product Manager: Câu chuyện này nói về cái gì, viết cho ai đọc, và điểm độc quyền (USP) của nó là gì?"

**Những gì cần bao gồm**:
- Tóm tắt bằng một câu duy nhất (Logline)
- Độc giả mục tiêu
- Xung đột cốt lõi (Mâu thuẫn lớn nhất)
- Các nhân vật chủ chốt
- Tiêu chí đánh giá sự thành công của tiểu thuyết

**Tại sao bước này quan trọng**:
- Trả lời rành mạch "Viết cho ai" và "Viết về cái gì"
- Cung cấp các tiêu chuẩn rõ ràng để đo lường
- Làm cái đích nhắm cho các bước triển khai sau

**Thời gian dự kiến**: 30-45 phút

**Các thẻ đánh dấu hệ thống**:
- `[Cần làm rõ]` - Đánh dấu các ý tưởng còn mập mờ
- `[Cốt lõi]` - Yêu cầu bất khả kháng
- `[Tùy chọn]` - Những tính năng/sự kiện thêm mắm dặm muối

### Bước 3: Làm rõ các quyết định then chốt

> "Chạy lệnh `/clarify` để giải quyết bất kỳ khuất mắc nào thông qua 5 câu hỏi sắc lẹm. AI sẽ đánh hơi các điểm mù trong Bản đặc tả của bạn và ép bạn đưa ra quyết định dứt khoát."

**Tại sao bước này quan trọng**: Mập mờ trong Kế Hoạch = Rác trong Bản Thảo.

**Quy trình thực hiện**:
- AI rà quét và phát hiện mâu thuẫn trong Bản đặc tả.
- Tạo ra tối đa 5 câu hỏi sát sườn.
- Người dùng trả lời tương tác, các câu trả lời sẽ dùng để update Bản đặc tả.
- Lưu lại lịch sử quyết định để truy vết sau này.

**Ví dụ về các câu hỏi điển hình**:
- "Động cơ sâu thẳm của nhân vật Nguyễn Ánh là báo thù cho gia tộc hay duy trì quyền lực đế vương?"
- "Nhịp độ câu chuyện là dồn dập nhiều cú twist, hay chậm rãi thiên về tâm lý?"
- "Kết cục sẽ là Đại đoàn tụ hay Bi kịch tàn nhẫn?"

**Thời gian dự kiến**: 10-15 phút

### Bước 4: Lên Kế Hoạch Sáng Tác

> "Sử dụng `/plan` để phác thảo cấu trúc chương hồi và các kỹ thuật sẽ áp dụng. Đây là lúc bạn thiết kế chi tiết 'How' – Làm thế nào để Bản đặc tả thành hình."

**Những gì cần thiết kế**:
- Chia nhỏ Chương và vạch các tuyến truyện đan xen.
- Phân bổ nhịp độ và áp lực căng thẳng (Tension).
- Lên sơ đồ cài cắm phục bút (Foreshadowing).
- Bản đồ phát triển Tâm lý Nhân vật (Character arcs).

**Tại sao bước này quan trọng**:
- Cụ thể hóa Bản đặc tả trừu tượng thành Kế hoạch thực thi.
- Lựa chọn phương pháp cấu trúc phù hợp (VD: 3 hồi, 7 bước).
- Cụ thể hóa nhân vật, cốt truyện, lore.

**Ví dụ về các kỹ thuật được chốt**:
- "Sử dụng Cấu trúc 7 điểm (Seven-Point Structure) để gia tăng sự dồn dập."
- "Triển khai cốt truyện Đa tuyến (Multi-POV) cho thấy sự phức tạp của Lục Quốc."
- "Sử dụng góc nhìn Hạn chế (Limited POV) để giấu kín mưu đồ."

**Thời gian dự kiến**: 45-60 phút

### Bước 5: Phân rã thành các Task công việc (Tasks)

> "Chạy lệnh `/tasks` để bóc tách Kế hoạch thành các hành động cụ thể, có phân cấp ưu tiên, có quản lý phụ thuộc (dependencies) và ước lượng thời gian."

**Các loại Task dự kiến**:
- Task viết thô (Drafting) các chương.
- Task hoàn thiện hồ sơ nhân vật.
- Task bồi đắp Worldbuilding (Lore).
- Task hiệu đính và điêu khắc câu chữ.

**Các thẻ Tracking**:
- `[P]` - Có thể thực thi song song (Parallel)
- `[Phụ thuộc:X]` - Phải chờ Task X hoàn thành
- `[Ưu tiên cao]` - Tiến độ sống còn

**Tại sao bước này quan trọng**:
- Chẻ nhỏ Núi công việc thành các Hòn đá để dễ dọn dẹp.
- Giúp người dùng biết nên làm cái gì trước, cái gì sau.
- Có thể sáng tác nhiều luồng cùng lúc mà không lo chệch ray.

**Thời gian dự kiến**: 20-30 phút

### Bước 6: Tiến hành Viết 📝

> "Bắt đầu gọi `/write` để khởi sự. Dựa trên Bản đặc tả và Bản kế hoạch, đây là lúc bạn sinh ra nội dung (Hoặc tự viết tay, hoặc yêu cầu AI hỗ trợ sườn)."

*(Lưu ý: Nếu Hiến pháp định nghĩa Tác giả là người viết chính, bước này Tác giả tự thi hành trên file Obsidian cá nhân và chỉ nhờ AI đưa gợi ý kỹ thuật giao tiếp/chuyển cảnh).*

**Chuyện gì ngầm xảy ra**:
- Các kỹ năng Thể loại (Genre skills) tự động bật.
- Bộ máy rà soát Tính nhất quán (Consistency checker) hoạt động ngầm.
- Phân tích nhịp độ và cảnh báo nếu Tác giả đi sai nhịp.

**Nguyên tắc kỷ luật**:
- Tuân thủ tuyệt đối Hiến pháp (`/constitution`).
- Không xa rời Kế hoạch (`/plan`).
- Giải quyết gọn gàng các Task (`/tasks`).
- Bám sát Đặc tả (`/specify`).

**Nhịp độ Khuyến nghị**:
- Viết 1-2 chương mỗi phiên (Session).
- Dừng lại ngẫm và review sau mỗi 3-5 chương.
- Giữ đà phóng tới trước, hạn chế sa đà vào việc bôi xóa tiểu tiết khi đang viết nháp.

### Bước 7: Kiểm định Chất lượng (Analyze)

> "Cứ sau 5 chương, chạy `/analyze` để rà soát lỗi logic, giữ chuẩn chất lượng và nắm bắt những thứ bất hợp lý từ trứng nước."

**Hai chế độ Kiểm định**:
- **Kiểm định Bộ khung** (Trước khi viết): Check xem Plan có hổng nát không.
- **Kiểm định Nội dung** (Sau khi viết): Check xem viết có lệch so với Plan không.

**Các trục đo lường**:
- Thượng tôn Hiến pháp (Có phá luật đã đề ra không?).
- Độ thỏa mãn Đặc tả (Có đạt được các Yêu cầu ban đầu không?).
- Lỗ hổng Logic (Thời gian xuyên không, nhân vật chẻ đôi, plot hole).
- Chất lượng Văn chương (Đo lường so với tiêu chuẩn đặt ra).

**Lịch trình kích hoạt**:
- Xong 3 chương đầu (Kiểm tra sớm xem có lạc lối không).
- Cách mỗi 5 chương (Khám sức khỏe định kỳ).
- Viết xong bản nháp 1 (Khám tổng quát).

## Sự tự động hóa của Hệ thống Skills

Khi di chuyển dọc theo hệ thống, các skill vệ tinh sẽ tự nhảy ra khi ngửi thấy mùi ngữ cảnh:

**Khi ở bước `/specify`**:
- Mùi "Lãng mạn" → Kích hoạt Skill Romance
- Mùi "Đấu trí/Âm mưu" → Kích hoạt Skill Mystery
- Mùi "Giả tưởng" → Kích hoạt Skill Fantasy

**Khi ở bước `/write`**:
- Bắt đầu gõ đối thoại → Kích hoạt Skill Dialogue Techniques
- Dựng cảnh đâm chém → Kích hoạt Skill Scene Structure
- Cứ viết là có lỗi → Skill Consistency Checker âm thầm giương mắt quan sát

**Triết lí xuyên suốt**:
- Guide này nắm trùm, kiểm soát không cho Tác giả lạc lối.
- Ép Tác giả đi theo lớp lang mà không nhảy bước.

## Cách AI phản ứng khi Tác giả đi chệch đường ray

Nếu Người dùng cố tình lách luật, xông thẳng vào viết mà không chịu lập Kế hoạch:

**Cảnh cáo nhẹ nhàng**:
> "Tôi thấy bạn đang vội vàng lao thẳng vào viết. Sức mạnh khủng khiếp nhất của hệ thống này nằm ở sự Lập Trình trước cơ mà? Bạn có muốn chạy `/constitution` và `/specify` trước để đào cái móng nhà thật sâu không? Chịu khổ lấp lỗ bây giờ, đoạn sau sẽ viết mướt lướt vô cùng."

**Nếu Tác giả vẫn bướng bỉnh**:
> "Okay, tôi hiểu – Bạn luôn có thể lên Kế hoạch sau. Nhưng hãy lưu ý: do bỏ qua `/specify` và `/plan`, bạn sẽ phải Tự Mình Rà Soát lại toàn bộ logic và tính nhất quán bằng tay ráng chịu nhé."

## Scale (Quy Cấp) Theo Kích Cỡ Tiểu Thuyết

### Truyện Giới hạn (1-3 Vạn chữ)

**Lược đồ Rút gọn**:
```
/specify → /clarify → /write → /analyze
```
**Trọng tâm**: Xác định Xung đột lõi và Cú Twist lớn.
**Thời gian rèn**: 1-2 ngày căng não.

### Truyện Dài (10-20 Vạn chữ)

**Lược đồ Chuẩn**:
```
Chạy đủ 7 bước không trượt phát nào.
```
**Trọng tâm**: Xẻ Task càng vụn càng tốt.
**Thời gian rèn**: 2-6 tháng.

### Trường thiên Cực Dài (50 Vạn chữ trở lên)

**Lược đồ Tuần hoàn**:
```
Lặp đi lặp lại đệ quy: plan → tasks → write → analyze
```
**Trọng tâm**: Kiểm định Tính Nhất Quán tới chết.
**Thời gian rèn**: 6-18 tháng.

## Trả lời Câu hỏi Phổ biến

### "Nhưng tôi có Dàn ý bằng tay rồi?"
> "Tuyệt! Vậy hãy nhét nó vào lệnh `/specify` để chuẩn hóa nó về form của Hệ thống máy. Bằng cách đó, tôi (AI) mới có thể đọc, hiểu, và giám sát nó tự động được chứ."
**Công thức**:
1. Đập dàn ý cũ vào.
2. Ép `/specify` gọt dũa lại.
3. Chạy `/clarify` lấp những kẽ hở.
4. Chạy `/plan` để đẩy ra technical blueprint.

### "Sao rườm rà thế? Tốn cả đống thời gian setup?"
> "1 tiếng setup bây giờ sẽ cứu bạn ròng rã 100 tiếng bôi xóa sửa lỗi logic ở chương 75. Bạn đang tạo ra 'Mã nguồn' (Source code) cho bộ tiểu thuyết của mình đấy. Lỗi ở đâu, vô Source code chắp vá lại, toàn bộ văn bản nhảy theo. Dám tay không bắt giặc không?"
**ROI (Lợi nhuận)**: Đảm bảo tính liền mạch, Quản lý thay đổi siêu tốc, Kiểm soát lượng thông tin khổng lồ tự động.

### "Tôi chỉ xài vài lệnh thôi được không?"
> "Được, nhưng hãy nhớ:
> - Không có `/specify` & `/plan` thì lấy cái quái gì để mà `/write` cho chuẩn?
> - Không có nội dung đã viết thì lấy gì để `/analyze`?
> Tối thiểu Vi Mô: `/constitution` → `/specify` → `/write/`"

*(Tip: Có thể lượt bỏ `/clarify` nếu bạn là vị thần logic, hoặc `/tasks` nếu bạn thích bay bổng).*

### "Nó có phá vỡ phong cách Freestyle của tôi không?"
- **Phong cách Planer (Người Lập Trình):** Sẽ nghiện cái này như điếu đổ.
- **Phong cách Pantser (Viết tới đâu hay tới đó):** Chỉ cần setup `/specify` thật mỏng, rồi xông lên Viết tự do.
- **Phong cách Hybrid (Lai):** Du di dọc đường.

## Bảng Hiển thị Tiến Độ Chớp Nhoáng (Status Tracking)

Với mỗi chu kỳ, AI sẽ hiện Radar check in như sau:

```
✅ /constitution  -- Đã duyệt
✅ /specify       -- Đã duyệt
✅ /clarify       -- Đã chốt
🔄 /plan          -- Đang vẽ...
⏸️ /tasks         -- Đang chờ
⏸️ /write         -- Đang chờ
⏸️ /analyze       -- Đang chờ
```

## Khớp Nối Với Các Skill Vệ Tinh Khác

**Tự Gọi Quân Cứu Viện:**
- Bế tắc tâm lý nhân vật → Kích hoạt Skill *Character Development*
- Bế tắc vì 10 chương rồi chưa uýnh nhau → Kích hoạt *Scene Structure*

**Sự Phối Hợp Tuyệt Đối:**
Mọi Skill đều quy chiếu về Workflow 7 bước này để biết bạn đang kẹt ở điểm mù nào.

## Giao Ý Thức Dành Riêng Cho Người Dùng

**Xuyên Suốt Cuộc Hành Trình:**
- Hệ thống AI sẽ nhắc bài liên tục.
- Hệ thống tự động gào thét nếu có mâu thuẫn (Consistency check).
- **Phân chia rạch ròi: Bạn sáng tạo nghệ thuật, AI xử lý đống bùn lầy của sự hỗn mang quản lý.**

**Bạn Luôn Là Lãnh Chúa Cao Nhất:**
- Bước nào thừa thải? Bấm Skip (Bỏ qua).
- Luật nào bất mãn? Cắt bỏ.
- AI không là cái đinh gì sất, AI chỉ là công cụ để phục vụ bản ngã tác phẩm của bạn.

---

**Nhắc nhớ:** Cái Workflow này không phải gông cùm – nó là **Bộ Cốt Thép**. Nó chịu tải toàn bộ áp lực kẽ hở logic, để tâm trí bạn hoàn toàn tĩnh lặng và xuất thần. Sau 1 tháng, bạn sẽ không bao giờ hiểu nổi ngày xưa mình viết chay kiểu gì mà sống được.

**Đã sẵn sàng chưa? Hãy phát nổ bắt đầu bằng lệnh `/constitution` nhé!**
