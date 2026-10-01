# Website — GitHub Pages (Two Egoes)

Trang tĩnh, không JavaScript, không theo dõi: `index.html`, `support.html`, `privacy.html`, `terms.html` × 7 ngôn ngữ
(`/`, `/vi/`, `/zh-hans/`, `/fr/`, `/pt/`, `/es/`, `/id/`), có `hreflang`, sáng/tối theo hệ thống.
Sinh lại: `python3 Scripts/build_publishing.py` (chữ ở `Scripts/web_copy.py`, email lấy từ `00_GLOBAL/FactoryOwner.json`).

## Bật GitHub Pages (Hồ làm tay)
1. Tạo repo `DLHkaizen/twoegoes` (public) trên GitHub.
2. Chép toàn bộ nội dung thư mục này vào gốc repo (kể cả `.nojekyll`, `shots/`, `icon.png`), commit, push.
3. Repo → Settings → Pages → Source: *Deploy from a branch* → Branch `main` / `(root)` → Save.
4. Đợi 1–2 phút, kiểm 4 URL trả **HTTP 200** (Golden Rule 15 §8 — không nộp App Store khi còn URL chết):
   - https://dlhkaizen.github.io/twoegoes/
   - https://dlhkaizen.github.io/twoegoes/support.html
   - https://dlhkaizen.github.io/twoegoes/privacy.html
   - https://dlhkaizen.github.io/twoegoes/terms.html
5. Sau đó sửa `websiteRule` của dòng 015 trong `06_REGISTRY/AppRegistry.json` (bỏ chữ "pending").

Nút App Store trên trang chủ đang là chỗ giữ chỗ — thay `href="#"` bằng link app sau khi app được duyệt.
