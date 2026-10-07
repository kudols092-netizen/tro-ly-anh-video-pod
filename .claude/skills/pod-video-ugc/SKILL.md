---
name: pod-video-ugc
description: Viết kịch bản và prompt Veo 3 (Google Flow) cho video UGC/creator demo sản phẩm POD/dropship, chia thành các cảnh 8 giây, giọng Mỹ tự nhiên, cho TikTok Shop, Reels/Meta Ads, Etsy, Amazon. Dùng khi anh Kiên muốn "video review", "video UGC", "video TikTok", "video quảng cáo", "hook".
---

# Video UGC / demo sản phẩm bằng Veo 3

## Bước 1 — Brief
Sản phẩm (xem ảnh gốc), kênh, độ dài mục tiêu (TikTok 15–30s = 2–4 cảnh), góc bán (quà tặng / mùa lễ / hài hước / tự thưởng), ngân sách credit Flow.

## Bước 2 — Chọn khung kịch bản
- **Hook – Show – Reason – CTA** (mặc định)
- **POV**: "POV: your bestie gets you a mug with your name on it"
- **Unboxing**: mở hộp → phản ứng → cận chi tiết in tên
- **Gift reaction**: người tặng quay người nhận mở quà (thoại do người tặng, không giả làm khách đã mua)
- **Problem → solution** (hàng dropship tiện ích)

Viết 3 hook khác nhau (≤ 2 giây, tiếng Anh Mỹ đời thường) để anh test A/B.

## Bước 3 — Bảng cảnh
Mỗi cảnh 8 giây: | # | Hình ảnh | Thoại (≤ 20 từ) | Âm thanh nền | Ghi chú |
Giữ **cùng một nhân vật**: mô tả nhân vật y hệt ở mọi cảnh, và tạo ảnh nhân vật trước bằng `pod-anh-nguoi-mau` để dùng làm "Ingredients"/frame đầu.

## Bước 4 — Prompt Veo cho từng cảnh (tiếng Anh)

```
Vertical 9:16 UGC-style smartphone video, handheld, slightly shaky, natural light.
Character: [mô tả cố định: a 28-year-old Latina woman, long dark wavy hair, pink oversized hoodie, gold hoop earrings].
Setting: [bối cảnh Mỹ: her small apartment kitchen, Halloween decorations, morning light].
Action: [hành động: she lifts the pink ghost mug toward the camera and turns it to show the name "Sophia" printed on it].
The mug matches the reference image exactly: cream body, pink inside and pink handle, printed ghost with leopard sunglasses, gold text "Boo-Jee". Print is flat, text must be legible.
She says, in a casual excited American voice: "[thoại]"
Audio: [quiet kitchen ambience, soft lo-fi music]. No subtitles, no on-screen text, no logos.
```

Quy tắc: không chữ trên màn hình trong prompt (chữ AI hay lỗi — thêm phụ đề sau bằng CapCut); thoại ngắn để khớp khẩu hình; 1 hành động chính mỗi cảnh.

## Bước 5 — Giao
Hook ×3 · bảng cảnh · prompt từng cảnh · caption + 5 hashtag · gợi ý phụ đề/nhạc khi ghép trong CapCut.
Nhắc: tag "AI-generated" khi đăng TikTok; thoại kiểu creator giới thiệu, **không** "I ordered this and…".
Lưu vào `output/<ten-san-pham>/video-ugc.md`.

## Hướng dẫn Flow
Profile TaoanhAI → Flow → New project → chọn Veo (Frames/Ingredients to video nếu có ảnh nhân vật + ảnh sản phẩm) → tỉ lệ 9:16 → dán prompt từng cảnh → tạo 2 bản/cảnh → chọn bản sản phẩm đúng nhất → dùng Scenebuilder hoặc tải về ghép CapCut.
