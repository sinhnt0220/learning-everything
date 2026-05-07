---
aliases:
  - "{{title}}"
tags:
  - type/moc
status: in-progress
priority: high
created: {{date}}
type: moc
project:
  - "[[{{title}} - MoC]]"
domain: "[[{{domain}}]]"
---

# 🎯 {{title}}

> [!info] Mục tiêu cốt lõi
> [Điền mục tiêu tối thượng của môn học này]

## 📡 HỆ THỐNG LIÊN KẾT (RADAR V4)

### 📚 Tư liệu liên quan (Literature)
```dataview
TABLE status AS "Trạng Thái", created AS "Ngày Tạo"
FROM -"00_Templates"
WHERE type = "literature" AND contains(file.outlinks, this.file.link)
SORT ASC
```

### 💎 Nội dung đã chưng cất (Permanent)
```dataview
TABLE status AS "Tiến độ", created as "Ngày Tạo"
FROM -"00_Templates"
WHERE type = "permanent" AND contains(file.outlinks, this.file.link)
SORT created ASC
```

### 🧠 Xưởng Đúc Kết (Synthesis)
```dataview
TABLE status AS "Tiến độ", created as "Ngày Tạo"
FROM -"00_Templates"
WHERE type = "synthesis" AND contains(file.outlinks, this.file.link)
SORT created ASC
```

---

## LỘ TRÌNH HUẤN LUYỆN (THE CURRICULUM)

### 🏛️ MODULE 1: [Tên Giai Đoạn]
*[Mục tiêu của giai đoạn]*
- [ ] [[Tên Module 1.1]] ⏳
  - **Fei Fei Feedback:** [AI sẽ ghi đè nhận xét rút gọn vào đây sau lệnh /complete-module]
- [ ] [[Tên Module 1.2]] (Chờ Start)

---

## 📜 DẤU ẤN TOÀN HÀNH TRÌNH (The Legacy)
- **Thành quả lớn nhất:** [Sẽ tổng hợp khi hoàn thành toàn bộ lộ trình]
- **Hành động thực tế:** [Kế hoạch vận hành vào thực tiễn]

---
## 📅 LỊCH SỬ HÀNH TRÌNH (Timeline)
- **{{date}}:** Khởi tạo lộ trình.
