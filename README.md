# Trợ lý Ảnh & Video POD

Bộ cấu hình Claude Code để tạo ảnh và video bán hàng POD/dropship cho thị trường Mỹ bằng Google Flow (Nano Banana, Veo, Omni), theo phong cách chân thật như ảnh khách hàng tự chụp.

## Gồm những gì
| File | Vai trò |
|---|---|
| `CLAUDE.md` | Vai trò trợ lý, thông số ảnh/video theo kênh (Etsy, Amazon, TikTok Shop, Meta Ads), nguyên tắc "chân thật", ranh giới bảo vệ shop |
| `.claude/skills/pod-anh-nguoi-mau` | Prompt ảnh người mẫu mặc/dùng sản phẩm, giữ nguyên thiết kế in |
| `.claude/skills/pod-video-ugc` | Kịch bản + prompt video UGC/creator demo, chia cảnh 8 giây |
| `.claude/skills/pod-anh-lifestyle` | Ảnh lifestyle/mockup và bộ ảnh listing theo từng kênh |
| `.claude/skills/pod-prompt-hang-loat` | Sinh prompt/hook hàng loạt cho nhiều sản phẩm, xuất CSV |
| `.mcp.json` | Playwright MCP (chế độ `--extension`) để Claude thao tác Google Flow trong Chrome profile `TaoanhAI` |

## Cài đặt
1. Clone repo, mở thư mục bằng Claude Code.
2. Cài tiện ích [Playwright Extension](https://chromewebstore.google.com/detail/playwright-extension/mmlmfjhmonkocbjadbfplnigmagldckm) vào Chrome profile dùng cho Flow, đăng nhập Google.
3. Nếu thư mục profile Chrome không phải `Default`/`Profile N`, sửa `PLAYWRIGHT_MCP_PROFILE_DIR_NAME` trong `.mcp.json` cho đúng tên thư mục.
4. Bỏ ảnh sản phẩm vào `Ảnh sản phẩm/`; kết quả được lưu ở `output/<ten-san-pham>/` (hai thư mục này không đưa lên git).
