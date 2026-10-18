我的影視資料庫 PWA

檔案：
- index.html：主要網頁，包含搜尋、篩選、排序、收藏、已觀看、本機儲存及 CSV 匯入／匯出
- manifest.webmanifest：PWA 安裝設定
- sw.js：Service Worker，快取介面以支援離線開啟
- icon.svg：App 圖示
- dramalist.csv：你提供的影視清單，部署後會嘗試自動載入

開始使用：
1. 將整個資料夾部署至支援 HTTPS 的靜態網站主機（例如 Cloudflare Pages、GitHub Pages 或其他 HTTPS 主機）。請保留所有檔案在同一資料夾。
2. 用瀏覽器打開部署後的網址。
3. 按「匯入 CSV」，選擇 dramalist.csv。
4. Android Chrome 可使用頁面「安裝 App」按鈕，或瀏覽器選單的「加到主畫面」。
5. 首次載入並匯入資料後，網頁介面會快取；資料及收藏儲存在該瀏覽器的本機儲存空間。

注意：
- 直接雙擊 index.html 可以在部分瀏覽器使用基本篩選，但 Service Worker／完整 PWA 安裝需要 localhost 或 HTTPS。
- 本機資料不會自動在手機與電腦之間同步。請用 CSV 匯出／匯入搬移資料。
- 請定期匯出備份；清除瀏覽器網站資料可能刪除收藏和觀看標記。
