# AGENTS.md - Cẩm Nang Xây Nhà

Áp dụng file này khi làm việc trong vault Obsidian:
`/home/node/.openclaw/workspace/cam-nang-xay-nha`

## Mục đích

Đây là Obsidian vault chứa **Cẩm Nang Xây Nhà** — kho kiến thức tích lũy về xây dựng nhà ở.

Mục tiêu khi làm việc trong vault này:
- cập nhật kiến thức mới vào đúng note
- giữ cấu trúc vault rõ ràng, nhất quán
- không làm hỏng format Obsidian hiện có
- ưu tiên bổ sung thông tin dựa trên dữ liệu người dùng cung cấp

## Ngôn ngữ và cách viết

- Luôn dùng **tiếng Việt**.
- Viết ngắn gọn, rõ ràng, thực dụng.
- Giữ định dạng phù hợp với Obsidian.
- Ưu tiên `[[wikilink]]` khi liên kết note nội bộ.
- Khi ghi nội dung có tính khuyến nghị:
  - dùng **in đậm** cho nội dung **nên dùng / nên làm**
  - dùng *in nghiêng* cho nội dung *không nên dùng / không nên làm*
- Thêm icon phù hợp nếu giúp nội dung dễ đọc hơn, ví dụ:
  - 🔧 mẹo kỹ thuật
  - ⚡ lưu ý quan trọng
  - 💡 gợi ý hay
  - 📐 kích thước, số đo
  - 🎨 thẩm mỹ
  - 💰 giá cả, ngân sách
  - 🌡️ nhiệt độ, độ ẩm
  - 🔩 vật liệu, linh kiện
  - 👷 kinh nghiệm từ thợ
  - ✅ / ❌ khuyến nghị nên / không nên

## Cấu trúc vault

Trang chủ:
- `🏠 Cẩm Nang Xây Nhà.md`

Các nhóm chính:
- `1-Chuan-bi/` — pháp lý, khảo sát, ngân sách, bản vẽ
- `2-Phan-tho/` — móng, kết cấu, tường, mái, cầu thang
- `3-He-thong-ME/` — điện, nước, điều hòa, PCCC
- `4-Hoan-thien/` — sơn, gạch, trần, cửa, chống thấm
- `5-Noi-that-Thiet-bi/` — bếp, phòng tắm, chiếu sáng, sàn, thiết bị
- `6-Nghiem-thu-Bao-tri/` — nghiệm thu, bảo hành, bảo trì

Mỗi nhóm có một file index riêng. Khi tạo note mới trong nhóm đã có, hãy cập nhật cả:
- file index của nhóm
- trang chủ `🏠 Cẩm Nang Xây Nhà.md`

## Nguồn sự thật

- Chỉ dùng thông tin từ:
  - nội dung đã có trong vault
  - dữ liệu người dùng vừa cung cấp trong chat
  - link/hình ảnh người dùng gửi kèm nếu được yêu cầu ghi nhận
- Không tự bịa facts, deadline, tiêu chuẩn, số liệu, hoặc kết luận không có căn cứ.
- Nếu thông tin chưa chắc chắn, ghi theo dạng ghi chú hoặc nêu rõ cần xác minh.

## Nguyên tắc chỉnh sửa

- Không xóa nội dung có sẵn, trừ khi người dùng yêu cầu rõ.
- Không đổi cấu trúc heading chỉ để “làm đẹp”.
- Ưu tiên **thêm đúng chỗ** thay vì viết lại toàn bộ note.
- Giữ nguyên frontmatter nếu đã có; chỉ cập nhật các trường cần thiết.
- Khi thêm kiến thức mới vào note hiện có, cập nhật `trang_thai` trong frontmatter từ `"chưa ghi"` sang `"đang cập nhật"` nếu phù hợp.
- Nếu một nội dung liên quan nhiều hạng mục, ghi vào hạng mục chính rồi thêm `[[wikilink]]` sang các note liên quan.
- Mặc định **không sửa file ngay** chỉ vì đã hiểu yêu cầu.
- Trước mọi thay đổi nội dung, phải tự làm đủ bước phân tích trước rồi mới hỏi xác nhận:
  - tìm file phù hợp nhất trong vault
  - đọc note mục tiêu
  - xác định luôn section cụ thể sẽ được cập nhật
  - chuẩn bị sẵn nội dung sẽ thêm hoặc note mới sẽ tạo
- Không dừng ở mức đề xuất mơ hồ theo thư mục hoặc nhóm chủ đề nếu vẫn có thể tìm được note cụ thể.
- Chỉ tiến hành sửa khi người dùng xác nhận rõ ràng.
- Nếu người dùng đã ra lệnh rất rõ theo kiểu “sửa luôn”, “cập nhật luôn”, “tạo luôn”, có thể thực hiện ngay, nhưng vẫn nên báo ngắn gọn mình sắp sửa file nào và section nào.

## Quy trình cập nhật note hiện có

Khi người dùng chia sẻ kinh nghiệm hoặc kiến thức mới:

1. Xác định file `.md` phù hợp nhất.
2. Đọc file đó trước khi phản hồi xác nhận.
3. Tìm đúng section cụ thể trong file.
4. Soạn sẵn nội dung mới sẽ thêm vào đúng section.
5. Hỏi xác nhận một lần, trừ khi người dùng đã yêu cầu làm ngay.
6. Thêm nội dung mới vào đúng section.
7. Nếu là kinh nghiệm thực tế, thêm ngày theo ngữ cảnh nếu có.
8. Cập nhật `trang_thai` trong frontmatter nếu cần.
9. Giữ nguyên format hiện có của note.

## Mapping section chuẩn

Khi cập nhật note, ưu tiên thêm vào đúng section sau:

- `## 📏 Quy chuẩn kỹ thuật`
  - dùng cho tiêu chuẩn, quy định, thông số kỹ thuật
- `## 🧱 Vật liệu phổ biến`
  - dùng cho vật liệu, ưu nhược điểm, ghi chú thực tế
  - nếu đang ở dạng bảng thì nối thêm hàng vào bảng thay vì đổi format
- `## ⚠️ Sai lầm thường gặp`
  - dùng cho lỗi cần tránh, bài học rút ra
- `## ✅ Mẹo kiểm tra & nghiệm thu`
  - dùng cho checklist, mẹo kiểm tra, tiêu chí đánh giá
- `## 📝 Kinh nghiệm thực tế`
  - dùng cho chia sẻ từ công trình, từ thợ, từ trải nghiệm thực tế

## Cách ghi kinh nghiệm thực tế

Khi thêm vào `## 📝 Kinh nghiệm thực tế`, dùng format như sau nếu note đang hỗ trợ kiểu này:

```md
### 📅 YYYY-MM-DD
- Nội dung kinh nghiệm thực tế
```

Ví dụ:

```md
### 📅 2026-04-05
- 👷 Đổ móng xong phải tưới nước (bảo dưỡng bê tông) ít nhất 7 ngày, không để bê tông khô quá nhanh sẽ dễ nứt.
```

## Tạo note mới khi chưa có chủ đề phù hợp

Khi nội dung người dùng chia sẻ chưa có file `.md` phù hợp:

### Trường hợp 1: vẫn thuộc một trong 6 nhóm chính

Tự tạo file `.md` mới trong thư mục phù hợp, sau đó:
- thêm `[[wikilink]]` vào file index của thư mục cha
- thêm `[[wikilink]]` vào `🏠 Cẩm Nang Xây Nhà.md`

### Trường hợp 2: nằm ngoài 6 nhóm lớn

Hỏi người dùng trước khi tạo thư mục mới, vì việc này ảnh hưởng đến cấu trúc tổng thể của vault.

## Template note mới

Khi cần tạo note mới trong các nhóm hiện có, dùng template sau:

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
| | | | |

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

## 🖼️ Hình ảnh minh hoạ

_Thêm ảnh minh hoạ khi có._

---

## 🔗 Tham khảo

_Link bài viết, video, sản phẩm liên quan._

---

**Quay lại:** [[<File index thư mục cha>]]
```

## Hình ảnh minh hoạ và link tham khảo

Khi người dùng chia sẻ hình ảnh hoặc đường link liên quan đến nội dung đang ghi:

### Hình ảnh

- Thêm vào section `## 🖼️ Hình ảnh minh hoạ`.
- Dùng cú pháp Obsidian:

```md
![[ten-file-anh.jpg]]
_Mô tả ngắn về ảnh_
```

### Link tham khảo

- Thêm vào section `## 🔗 Tham khảo`.
- Dùng cú pháp Markdown:

```md
- [Tên bài viết / video](URL) — mô tả ngắn
```

### Nếu note chưa có section tương ứng

- Tạo thêm section đó ngay trước dòng `**Quay lại:**`.

## Khi làm việc với file có sẵn

Trước khi sửa note:
- đọc note mục tiêu
- giữ nguyên cấu trúc hiện có nếu nó đã hợp lý
- ưu tiên patch nhỏ, đúng chỗ
- tránh viết lại cả file nếu chỉ cần thêm vài dòng

## Không được làm

- Không bịa thông tin ngoài dữ liệu có sẵn.
- Không xóa note hoặc đổi tên hàng loạt nếu chưa được yêu cầu.
- Không tự tạo thư mục lớn mới khi chưa hỏi người dùng.
- Không phá vỡ cấu trúc heading, bảng, frontmatter chỉ vì muốn chuẩn hóa.

## Workflow đề xuất trong chat mới

Khi được giao việc liên quan vault này, hãy làm theo thứ tự:
1. xác định note hoặc chủ đề người dùng muốn cập nhật
2. tìm file phù hợp nhất trong vault
3. đọc file đó trước khi sửa
4. xác định luôn section cụ thể sẽ cập nhật
5. soạn sẵn nội dung dự kiến thêm
6. đề xuất kế hoạch sửa thật ngắn gọn, nêu rõ file đích, section đích, và nội dung sẽ thêm
7. chờ người dùng xác nhận
8. chỉnh sửa tối thiểu nhưng đúng vị trí
9. nếu tạo note mới, cập nhật đầy đủ các trang index liên quan
10. báo lại ngắn gọn đã sửa file nào và thêm gì

## Mẫu phản hồi an toàn trước khi sửa

Khi chưa có xác nhận, ưu tiên trả lời theo dạng:
- `Mình sẽ cập nhật file <path>`
- `Section sẽ sửa: <tên section>`
- `Nội dung sẽ thêm: <tóm tắt ngắn hoặc đoạn dự kiến thêm>`
- `Nếu bạn đồng ý, mình sẽ sửa luôn.`
