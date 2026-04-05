---
name: cam-nang-xay-nha
description: Làm việc với Obsidian vault Cẩm Nang Xây Nhà tại /home/node/.openclaw/workspace/cam-nang-xay-nha. Dùng khi người dùng muốn cập nhật, phân loại, ghi thêm kinh nghiệm, tạo note mới, thêm link hoặc hình ảnh vào vault này. Khi được gọi qua slash command /cam_nang_xay_nha, trước hết phải xác nhận workspace, vault, và file AGENTS.md đang áp dụng; sau đó đề xuất file/section sẽ sửa trước khi chỉnh nội dung.
user-invocable: true
---

# Cam Nang Xay Nha

Skill này áp dụng cho vault:
- `/home/node/.openclaw/workspace/cam-nang-xay-nha`

## Trước khi làm gì

Luôn xác nhận ngắn gọn:
- workspace hiện tại: `/home/node/.openclaw/workspace`
- vault đang làm việc: `/home/node/.openclaw/workspace/cam-nang-xay-nha`
- file rule đang áp dụng: `/home/node/.openclaw/workspace/cam-nang-xay-nha/AGENTS.md`

Sau đó đọc file sau trước khi đề xuất thay đổi:
- `/home/node/.openclaw/workspace/cam-nang-xay-nha/AGENTS.md`

## Hành vi mặc định

- Mặc định **không sửa file ngay**.
- Với yêu cầu kiểu slash command hoặc yêu cầu ngắn, **không dừng ở mức phỏng đoán thư mục/nhóm note**.
- Phải tự làm bước phân tích trước khi hỏi lại người dùng:
  1. tìm note mục tiêu phù hợp nhất trong vault
  2. đọc note đó
  3. xác định luôn **section cụ thể** sẽ cập nhật
  4. soạn sẵn nội dung dự kiến thêm
- Chỉ sau đó mới hỏi xác nhận một lần.
- Nếu người dùng ra lệnh rất rõ như “sửa luôn”, “cập nhật luôn”, “tạo luôn”, có thể tiến hành ngay, nhưng vẫn phải báo ngắn gọn file mục tiêu và section mục tiêu trước khi sửa.

## Cách phản hồi khi được gọi

Ưu tiên phản hồi theo mẫu:

- `Workspace: /home/node/.openclaw/workspace`
- `Vault: /home/node/.openclaw/workspace/cam-nang-xay-nha`
- `AGENTS.md áp dụng: /home/node/.openclaw/workspace/cam-nang-xay-nha/AGENTS.md`
- `File sẽ sửa: ...`
- `Section sẽ sửa: ...`
- `Nội dung sẽ thêm: ...`
- `Nếu bạn đồng ý, mình sẽ sửa luôn.`

Không dùng kiểu trả lời mơ hồ như “mình đề xuất nhóm 4 hoặc 5”, trừ khi thực sự chưa tìm được note phù hợp sau khi đã tìm trong vault.

## Khi thực hiện chỉnh sửa

- Đọc note mục tiêu trước.
- Giữ nguyên format Obsidian hiện có.
- Ưu tiên patch nhỏ, đúng vị trí.
- Tuân thủ đầy đủ rule trong file AGENTS.md của vault.

## Nếu người dùng chỉ nhập ngắn sau slash command

Nếu người dùng gọi dạng:
- `/cam_nang_xay_nha <nội dung>`

thì hiểu `<nội dung>` là yêu cầu liên quan đến vault này, và phải xử lý theo thứ tự:
1. xác nhận workspace/vault/AGENTS.md
2. tìm file mục tiêu phù hợp nhất trong vault
3. đọc file đó trước
4. xác định **section cụ thể** sẽ sửa theo mapping section chuẩn hoặc cấu trúc thực tế của note
5. viết sẵn nội dung dự định thêm
6. hỏi xác nhận một lần trước khi sửa, trừ khi người dùng đã yêu cầu làm ngay

Chỉ nếu sau khi tìm trong vault mà vẫn chưa có note phù hợp, mới đề xuất tạo note mới và nêu rõ note mới sẽ nằm ở đâu.
