---
name: pod-prompt-hang-loat
description: Sinh hàng loạt prompt ảnh/video và hook cho nhiều sản phẩm POD/dropship cùng lúc (nhiều thiết kế, nhiều tên cá nhân hóa, nhiều mùa lễ, nhiều kênh), xuất ra file CSV để anh Kiên dán lần lượt vào Google Flow. Dùng khi anh nói "hàng loạt", "nhiều sản phẩm", "cả bộ sưu tập", "100 prompt", "lịch content".
---

# Prompt & hook hàng loạt

## Đầu vào
- Thư mục ảnh (mặc định `Ảnh sản phẩm/`) hoặc danh sách sản phẩm anh dán vào.
- Kênh, số lượng ảnh/video mỗi sản phẩm, dịp lễ (xem lịch dưới).

## Cách làm
1. Xem từng ảnh sản phẩm, ghi 1 dòng mô tả cố định (loại, màu, chữ in, chủ đề) — dùng lại y hệt trong mọi prompt của sản phẩm đó để giữ đúng thiết kế.
2. Xác định khách mục tiêu + góc bán cho mỗi sản phẩm.
3. Sinh prompt theo mẫu trong các skill `pod-anh-nguoi-mau`, `pod-anh-lifestyle`, `pod-video-ugc`; xoay vòng người mẫu (tuổi/sắc tộc/dáng), bối cảnh, góc máy để không lặp.
4. Viết hook/caption tiếng Anh Mỹ, mỗi sản phẩm ≥3 hook khác góc (quà tặng, hài hước, tự thưởng).
5. Ghi file `output/hang-loat-<yyyy-mm-dd>.csv` (UTF-8 có BOM để Excel đọc đúng tiếng Việt), các cột:
   `san_pham, kenh, loai (anh/video), concept_vi, ti_le, prompt_en, hook_en, caption_en, hashtags, trang_thai`
   `trang_thai` để trống — anh đánh dấu "xong" khi đã tạo trên Flow.
6. Báo tóm tắt: số sản phẩm, số prompt, gợi ý thứ tự làm (sản phẩm nào sát mùa làm trước).

## Lịch mùa vụ Mỹ (ưu tiên content trước dịp 4–6 tuần)
Valentine (14/2) · St. Patrick (17/3) · Easter · Mother's Day (CN thứ 2 tháng 5) · Father's Day (CN thứ 3 tháng 6) · 4th of July · Back to School (8) · Halloween (31/10) · Thanksgiving (thứ 5 thứ 4 tháng 11) · Black Friday/Cyber Monday · Christmas · Teacher/Nurse appreciation weeks (5).

## Lưu ý
- Không lặp đúng một prompt cho nhiều sản phẩm — Meta/TikTok phạt creative trùng lặp.
- Cá nhân hóa: dùng tên Mỹ phổ biến theo nhóm tuổi khách (vd. 25–40: Emily, Jessica, Ashley, Madison, Sophia).
- Giữ các ranh giới trong CLAUDE.md (không review giả, gắn nhãn AI, không IP có bản quyền).
