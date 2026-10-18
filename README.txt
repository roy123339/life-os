LIFE OS v1.0 — 個人自用 PWA

功能：每日任務點數、日記（照片與自訂獎勵）、自訂商城（商品照片）、點數收支、JSON 完整備份。

Windows 本機測試：
1. 安裝 Python（或使用 VS Code Live Server）。
2. 在本資料夾開啟終端機，執行 python -m http.server 8000
3. 電腦瀏覽器開啟 http://localhost:8000

iPhone 安裝：
1. 建立免費 GitHub 帳號，新增公開 repository（例如 life-os）。
2. 上傳 index.html、app.js、sw.js、manifest.webmanifest、icon.svg 到儲存庫根目錄。
3. Settings > Pages > Deploy from a branch > main / root > Save。
4. 等待 GitHub Pages 公布 HTTPS 網址（通常 https://帳號.github.io/life-os/）。
5. iPhone Safari 開啟網址 > 分享 > 加入主畫面。

重要：
- 資料存在瀏覽器 localStorage，照片會壓縮成 JPEG 並一起儲存。容量有限，不適合大量照片。
- 請定期從「設定 > 匯出完整備份」保存 JSON；清除網站資料會失去資料。
- GitHub Pages 的程式碼公開，但個人日記與照片不會自動上傳到 GitHub；它們保存在使用裝置的瀏覽器儲存空間。
- 目前僅當日寫日記才會獲得獎勵；補寫歷史日記不補發點數。
- 同一任務每天只能領一次；日記預設每天一次，可在設定中更改。
