---
name: pod-anh-nguoi-mau
description: Tạo prompt Nano Banana (Google Flow) để ra ảnh người mẫu Mỹ chân thật đang mặc áo/hoodie hoặc cầm/dùng cốc, decor, quà cá nhân hóa, hàng dropship — giữ nguyên thiết kế in. Dùng khi anh Kiên muốn "ảnh người mẫu", "model mặc áo", "người cầm cốc", "ảnh khách dùng sản phẩm".
---

# Ảnh người mẫu dùng sản phẩm thật

## Bước 1 — Thu thập
- Ảnh sản phẩm/design gốc (trong `Ảnh sản phẩm/`). Mở xem để mô tả đúng: loại sản phẩm, màu nền, màu phụ (lòng cốc, tay cầm, màu áo), chữ in, chủ đề/dịp.
- Kênh đăng (quyết định tỉ lệ khung, xem bảng trong CLAUDE.md). Không nói → làm 4:5 (dùng được Meta + Etsy crop).
- Khách hàng mục tiêu: ai mua, mua cho ai (vd. phụ nữ 25–40 thích Halloween "girly", mua tặng bạn thân).
Nếu thiếu, tự suy luận từ sản phẩm rồi nêu giả định, không hỏi dồn.

## Bước 2 — Chọn 3–5 concept
Mỗi concept = **Người mẫu** (tuổi, sắc tộc, dáng, trang phục hợp mùa) + **Hành động** tự nhiên + **Bối cảnh Mỹ** + **Góc máy** + **Ánh sáng**.
Ưu tiên: một concept "selfie gương/điện thoại", một concept "candid người khác chụp", một concept "cận tay + sản phẩm".

## Bước 3 — Prompt mẫu (tiếng Anh)

```
Use the attached product image as the exact reference.
A candid smartphone photo of [người mẫu: a 30-year-old woman with messy blonde bun, oversized cream knit sweater]
[hành động: holding the mug with both hands, smiling at someone off-camera]
in [bối cảnh: a cozy suburban American kitchen decorated for Halloween, small pumpkins on the counter].
The [sản phẩm: ceramic mug] is clearly visible, facing the camera, taking about 30% of the frame.
Keep the printed design, text and colors exactly as in the reference image. Do not redraw or alter the text.
The print is flat on the surface (no real embossing).
Shot on iPhone, handheld, natural window light, soft shadows, slight grain, realistic skin texture, no retouching.
Aspect ratio [4:5].
```

Áo/hoodie: thay dòng sản phẩm bằng "wearing the [màu] [t-shirt/hoodie] with the printed design centered on the chest, natural fabric wrinkles, the print follows the fabric folds".

## Bước 4 — Giao cho anh Kiên
Với mỗi concept: tên concept (tiếng Việt) · prompt (khối code) · kênh phù hợp.
Kèm hướng dẫn Flow: mở profile TaoanhAI → Flow → tạo ảnh (Nano Banana) → tải ảnh sản phẩm làm tham chiếu → dán prompt → tạo 2–4 biến thể → chọn ảnh chữ in đúng nhất.

Checklist duyệt ảnh: chữ/tên đúng chính tả · màu sản phẩm đúng · tay đủ 5 ngón, cầm tự nhiên · sản phẩm không bị méo · không có logo lạ.

Lưu prompt vào `output/<ten-san-pham>/anh-nguoi-mau.md`.

## Ví dụ: cốc "Boo-Jee" ghost (Halloween, cá nhân hóa tên)
Khách: phụ nữ 22–40, phong cách "boujee/girly Halloween". Concept gợi ý:
1. Cô gái uống cà phê sáng bên cửa sổ, áo len hồng, ngoài trời lá vàng.
2. Hai cô bạn tặng quà nhau ở quán cafe, một người mở hộp thấy cốc có tên mình.
3. Cận tay sơn móng màu nude cầm cốc, nền bàn làm việc có laptop và nến bí ngô.
4. Selfie gương phòng ngủ trang trí Halloween hồng, giơ cốc lên cạnh mặt.
