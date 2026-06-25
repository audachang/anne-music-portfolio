# 張安耘 ‧ 音樂歷程網站 (Anne's Music Journey)

靜態個人音樂作品集網站，供 GitHub Pages 託管於 `audachang.github.io`。

## 檔案結構

```
docs/
├── index.html                      # 主頁（單頁式網站）
├── .nojekyll                       # 讓 GitHub Pages 直接服務檔案，不經 Jekyll 處理
└── images/
    └── competitions/               # 比賽獎盃照片（5 張）
```

## 部署到 audachang.github.io

此網站要成為主網域 `https://audachang.github.io`，需放在名為
**`audachang.github.io`** 的 repository。兩種做法擇一：

### 做法 A：放在 repo 根目錄（最簡單）
1. 建立（或使用既有的）repository：`audachang.github.io`
2. 將 `docs/` 內的**所有檔案**複製到 repo 的**根目錄**。
3. `git add . && git commit -m "Anne music site" && git push`
4. Settings → Pages → Source 選 `main` 分支、資料夾 `/ (root)`。
5. 數分鐘後造訪 `https://audachang.github.io`。

### 做法 B：保留 docs/ 子資料夾
1. 將整個 `docs/` 資料夾推到 `audachang.github.io` repo。
2. Settings → Pages → Source 選 `main` 分支、資料夾 `/docs`。
3. 造訪 `https://audachang.github.io`。

> 若想放在子路徑（例如 `audachang.github.io/anne-music`），
> 則建立另一個名稱的 repo（如 `anne-music`），啟用 Pages 即可，網址會是
> `https://audachang.github.io/anne-music/`。

## 待補內容（可自行編輯 index.html）

- **演奏影片**：在「鋼琴」與「單簧管」區塊有預留的影片欄位，
  搜尋 `影片連結待補`，把 `media-card` 內容換成實際的 YouTube／影片連結即可。
  例：
  ```html
  <a class="btn btn-gold" href="https://youtu.be/XXXX" target="_blank" rel="noopener">▶ 觀看演奏</a>
  ```
- **獎項日期**：「古典鋼琴獨奏國際音樂大賽 第一名」目前標示「近年」，
  確認年份後可在 `index.html` 的 `<div class="year">` 修改。

## 資料來源

- Yamaha 課程階段：台灣山葉音樂官方網站 <https://www.yamahamusic.tw/yms/course>
- 獎項資訊：依專案 `competitions/photos/` 內獎盃／獎牌照片整理
- 完整比賽相簿：SmugMug <https://www.smugmug.com/app/organize/For-Sharing/Annes-music-competitions>
