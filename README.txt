# 地盤改良樁現場施工紀錄 App — PWA 版

這是一個可安裝到 Android / iPhone 主畫面的 PWA。

## 重要
PWA 不能直接用手機檔案管理員開啟 `index.html` 後就安裝。
必須放在 HTTPS 網站（或 localhost）上，Service Worker 才能工作。

## 最簡單部署
可把本資料夾全部上傳到任何支援 HTTPS 的靜態網站主機。
例如 GitHub Pages、Cloudflare Pages、Netlify 等。

上線後：
1. 用手機 Chrome / Safari 開啟網站。
2. Android Chrome：選單 →「新增至主畫面／安裝 App」。
3. iPhone Safari：分享 →「加入主畫面」。
4. 從桌面圖示開啟後會以獨立 App 介面執行。

## 功能
- 本地工程圖載入
- Leaflet 圖面縮放、拖曳
- 樁位建檔 1、2、3...
- 機台1：A1、A2...
- 機台2：B1、B2...
- 施工資料輸入
- 已完成樁點擊可防呆復原
- LocalStorage 保存資料
- CSV 匯出
- PWA Service Worker 快取
- 桌面獨立 App 顯示

注意：Leaflet 目前從 unpkg CDN 載入，因此第一次開啟需要網路；之後瀏覽器會依快取情況提供離線使用。
