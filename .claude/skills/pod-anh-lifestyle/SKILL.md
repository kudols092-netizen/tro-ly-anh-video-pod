---
name: pod-anh-lifestyle
description: Tạo prompt Nano Banana (Google Flow) cho ảnh lifestyle/mockup sản phẩm POD/dropship và trọn bộ ảnh listing theo từng kênh (Etsy, Amazon, TikTok Shop, Shopify/Meta). Dùng khi anh Kiên cần "ảnh listing", "mockup", "ảnh lifestyle", "ảnh nền trắng Amazon", "bộ ảnh sản phẩm".
---

# Ảnh lifestyle & bộ ảnh listing

## Bộ ảnh chuẩn (chọn theo kênh, xem thông số trong CLAUDE.md)
| # | Ảnh | Etsy | Amazon | TikTok | Meta |
|---|---|---|---|---|---|
| 1 | Hero: sản phẩm trong bối cảnh đẹp, rõ thiết kế | ✔ thumbnail | — | ✔ | ✔ |
| 2 | Nền trắng tinh, không chữ/props | tuỳ | ✔ ảnh chính bắt buộc | — | — |
| 3 | Cận chi tiết in (chất lượng in, tên cá nhân hóa) | ✔ | ✔ | ✔ | — |
| 4 | Người dùng (gọi skill `pod-anh-nguoi-mau`) | ✔ | ✔ | ✔ | ✔ |
| 5 | Kích thước/so sánh (cốc cạnh tay, áo trên móc + thước) | ✔ | ✔ | — | — |
| 6 | Quà tặng: hộp quà, thiệp, dịp lễ | ✔ | ✔ | ✔ | ✔ |
| 7 | Biến thể: các tên/màu khác nhau xếp cạnh nhau (cá nhân hóa) | ✔ | ✔ | — | ✔ |

Chữ marketing ("Personalized Gifts", "Fast Shipping US", bảng size) **không** nhờ AI viết — thêm sau bằng Canva/Photoshop. Amazon ảnh chính tuyệt đối không có chữ.

## Prompt mẫu

Hero / lifestyle:
```
Use the attached product image as the exact reference.
A realistic lifestyle photo of the [sản phẩm] placed on [bề mặt: a worn oak kitchen table]
in [bối cảnh Mỹ theo mùa: a cozy home in October, small white pumpkins, a knit blanket, warm fairy lights softly blurred in background].
Morning window light from the left, natural soft shadows, shallow depth of field, shot on iPhone 15 Pro, realistic, not overly styled.
Keep the printed design, text and colors exactly as in the reference image. Do not redraw or alter the text. Print is flat on the surface.
No added text, no logos, no watermark. Aspect ratio [1:1].
```

Nền trắng Amazon:
```
Use the attached product image as the exact reference.
Professional e-commerce product photo of the [sản phẩm] on a pure white background (RGB 255,255,255),
product centered and filling about 85% of the frame, [góc: three-quarter view with handle on the right], soft even studio lighting, subtle natural contact shadow.
Keep the printed design, text and colors exactly as in the reference image. No props, no text, no logos. Aspect ratio 1:1.
```

Cận chi tiết: "Extreme close-up macro photo of the printed name '[Tên]' on the [sản phẩm], showing print sharpness and [ceramic gloss / cotton fabric texture]…"

Cá nhân hóa — biến thể tên: tạo 1 ảnh/tên rồi ghép, hoặc "three identical mugs side by side, each printed with a different name: '[Tên1]', '[Tên2]', '[Tên3]', same design otherwise" (kiểm tra kỹ chính tả).

## Giao
Danh sách ảnh theo kênh anh chọn · prompt từng ảnh · việc cần làm sau (thêm chữ, crop).
Hướng dẫn Flow: profile TaoanhAI → Flow → tạo ảnh (Nano Banana) → đính ảnh sản phẩm gốc → dán prompt → chọn tỉ lệ → tạo 4 bản → tải bản tốt nhất.
Lưu vào `output/<ten-san-pham>/bo-anh-listing.md`.
