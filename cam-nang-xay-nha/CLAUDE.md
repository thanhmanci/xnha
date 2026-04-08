# Hướng dẫn cho Claude Cowork

## Mục đích
Đây là Obsidian vault chứa **Cẩm Nang Xây Nhà** — tài liệu tích lũy kiến thức xây dựng nhà ở.

## Cấu trúc thư mục

```
🏠 Cẩm Nang Xây Nhà.md      ← Trang chủ (Map of Content)
1-Chuan-bi/                   ← Pháp lý, khảo sát, ngân sách, bản vẽ
2-Phan-tho/                   ← Móng, kết cấu, tường, mái, cầu thang
3-He-thong-ME/                ← Điện, nước, điều hòa, PCCC
4-Hoan-thien/                 ← Sơn, gạch, trần, cửa, chống thấm
5-Noi-that-Thiet-bi/          ← Bếp, phòng tắm, chiếu sáng, sàn
6-Nghiem-thu-Bao-tri/         ← Nghiệm thu, bảo hành, bảo trì
```

## Quy tắc cập nhật

Khi người dùng chia sẻ kinh nghiệm hoặc kiến thức mới:

1. **Xác định hạng mục** — Đọc nội dung và tìm file `.md` phù hợp nhất
2. **Tìm đúng mục trong file** — Mỗi file có các section:
   - `📏 Quy chuẩn kỹ thuật` → cho tiêu chuẩn, quy định
   - `🧱 Vật liệu phổ biến` → cho thông tin vật liệu (thêm vào bảng)
   - `⚠️ Sai lầm thường gặp` → cho lỗi cần tránh
   - `✅ Mẹo kiểm tra & nghiệm thu` → cho cách kiểm tra
   - `📝 Kinh nghiệm thực tế` → cho ghi chú tự do, kinh nghiệm từ công trình
3. **Thêm nội dung** — Ghi vào đúng section, thêm ngày tháng nếu là kinh nghiệm thực tế
4. **Cập nhật trạng thái** — Đổi `trang_thai` trong frontmatter từ `"chưa ghi"` sang `"đang cập nhật"`
5. **Giữ format** — Không thay đổi cấu trúc heading, chỉ thêm nội dung vào

## Ví dụ

Người dùng nói: "Hôm nay thợ bảo đổ móng xong phải tưới nước ít nhất 7 ngày"
→ Mở file `2-Phan-tho/Móng.md`
→ Thêm vào section `📝 Kinh nghiệm thực tế`:
```
### 📅 2026-04-05
- Đổ móng xong phải tưới nước (bảo dưỡng bê tông) ít nhất 7 ngày, không để bê tông khô quá nhanh sẽ nứt
```

## Tạo node mới khi chủ đề chưa có file

Khi người dùng chia sẻ nội dung **không có file `.md` phù hợp** trong thư mục hiện tại:

1. **Nếu thuộc một trong 6 thư mục cha đã có** → Tự động tạo file `.md` mới trong thư mục đó với cấu trúc section chuẩn (giống các file khác), sau đó:
   - Thêm `[[link]]` vào file index của thư mục cha (ví dụ `⚡ Hệ Thống M&E.md`)
   - Thêm `[[link]]` vào trang chủ `🏠 Cẩm Nang Xây Nhà.md`

2. **Nếu hoàn toàn nằm ngoài 6 nhóm lớn** → Hỏi người dùng trước khi tạo thư mục mới, vì đây là quyết định ảnh hưởng đến cấu trúc tổng thể của vault.

### Cấu trúc chuẩn cho file `.md` mới

```markdown
---
tags: []
category: "<Tên thư mục cha>"
trang_thai: "đang cập nhật"
---

# <Tên chủ đề>

> <Thư mục cha> / <Tên chủ đề>

---

## 📏 Quy chuẩn kỹ thuật

_Ghi lại các tiêu chuẩn, quy chuẩn xây dựng liên quan._

-

---

## 🧱 Vật liệu phổ biến

| Vật liệu | Ưu điểm | Nhược điểm | Ghi chú |
|-----------|----------|------------|---------|
|           |          |            |         |

---

## ⚠️ Sai lầm thường gặp

_Những lỗi hay mắc phải, bài học từ thực tế._

1.

---

## ✅ Mẹo kiểm tra & nghiệm thu

_Cách kiểm tra chất lượng, checklist nghiệm thu._

- [ ]

---

## 📝 Kinh nghiệm thực tế

_Ghi chú tự do từ công trình, từ thợ, từ học hỏi._

### 📅

-

---

---

## 🖼️ Hình ảnh minh hoạ

_Thêm ảnh minh hoạ khi có._

---

## 🔗 Tham khảo

_Link bài viết, video, sản phẩm liên quan._

---

**Quay lại:** [[<File index thư mục cha>]]
```

## Hình ảnh minh hoạ & Link tham khảo

Khi người dùng chia sẻ **hình ảnh** hoặc **đường link** liên quan đến nội dung đang ghi:

1. **Hình ảnh minh hoạ** → Thêm vào section `🖼️ Hình ảnh minh hoạ` ở cuối file (trước dòng "Quay lại"), dùng cú pháp Obsidian:
   ```
   ## 🖼️ Hình ảnh minh hoạ
   ![[tên-file-ảnh.jpg]]
   _Mô tả ngắn về ảnh_
   ```

2. **Link tham khảo** (video YouTube, bài viết, sản phẩm...) → Thêm vào section `🔗 Tham khảo` ở cuối file (trước dòng "Quay lại"), dùng cú pháp Markdown:
   ```
   ## 🔗 Tham khảo
   - [Tên bài viết / video](URL) — mô tả ngắn
   ```

3. **Nếu section chưa tồn tại trong file** → Tạo thêm section đó ngay trước dòng `**Quay lại:**`

4. **Cập nhật template chuẩn** — Các file mới tạo phải bao gồm sẵn 2 section này.

## Lưu ý
- Luôn dùng tiếng Việt
- Thêm tag phù hợp vào frontmatter nếu có từ khóa mới
- Nếu kinh nghiệm liên quan đến nhiều hạng mục, ghi vào hạng mục chính và thêm `[[link]]` đến hạng mục liên quan
- Không xóa nội dung có sẵn, chỉ thêm mới
- **Định dạng khuyến nghị:** Khi ghi nội dung có tính chất khuyến nghị, áp dụng nhất quán:
  - **In đậm** → những gì **nên dùng / nên làm**
  - *In nghiêng* → những gì *không nên dùng / không nên làm*
- **Thêm icon thông minh:** Khi ghi nội dung vào bất kỳ section nào, chọn icon phù hợp với ngữ cảnh để ghi chú sinh động và dễ đọc hơn. Ví dụ:
  - 🔧 cho mẹo kỹ thuật, cách làm
  - ⚡ cho lưu ý quan trọng, cần chú ý ngay
  - 💡 cho ý tưởng, gợi ý hay
  - 📐 cho kích thước, số đo, công thức tính
  - 🎨 cho màu sắc, thẩm mỹ, thiết kế
  - 💰 cho giá cả, chi phí, ngân sách
  - 🌡️ cho nhiệt độ, độ ẩm, khí hậu
  - 🔩 cho vật liệu, linh kiện, phụ kiện
  - 👷 cho kinh nghiệm từ thợ
  - ✅ / ❌ cho khuyến nghị nên/không nên
