英文能力評估小遊戲（手機可安裝版 PWA）

✅ 這是一個 PWA（可安裝到手機主畫面、離線可用）
📦 你現在拿到的是一個資料夾（index.html + manifest + sw.js + icons）

【重要：要能安裝，必須用「HTTPS 網址」開啟】
- 電腦本機 localhost 可以，但手機連同一台電腦的 127.0.0.1 不行
- 最推薦：GitHub Pages / Netlify / Cloudflare Pages 其中一個（免費）

────────────────────────────────────
A. 最簡單（推薦）：GitHub Pages
1) 在 GitHub 建一個新 Repo（例如 english-quiz-pwa）
2) 把這個資料夾裡的所有檔案上傳到 Repo 根目錄
3) Repo → Settings → Pages → Source 選擇 Deploy from a branch
4) Branch 選 main / root → Save
5) 等它產生網址（https://xxxxx.github.io/english-quiz-pwa/）
6) 用手機打開這個網址

Android（Chrome）：
- 右上角 ⋮ → 「安裝應用程式」或「加入主畫面」

iPhone（Safari）：
- 分享按鈕 → 「加入主畫面」

────────────────────────────────────
B. 本機測試（電腦）
1) 用 VS Code 開資料夾
2) 用 Live Server 開啟（或：python -m http.server 5500）
3) 用瀏覽器開 http://localhost:5500

※ 手機要安裝仍需要 HTTPS，所以正式使用請走 A.

────────────────────────────────────
C. 常見問題
- 看不到「安裝」：通常是你不是 HTTPS、或 service worker 沒成功註冊
- iOS 沒有「安裝」字樣：請用 Safari 的「加入主畫面」
