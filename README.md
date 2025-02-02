# 網頁切版直播班 Vite 範例 - Bootstrap 版本

## Node.js 版本
- 專案的 Node.js 版本需為 **v16** 以上。
- 查看自己版本的指令：`node -v`

## 指令列表
- `npm install`  
  安裝所有相依的套件。  
  *說明*：在初次下載該範例專案後，請使用 `npm install` 來安裝所需的套件。

- `npm run dev`  
  啟動開發模式並自動開啟瀏覽器。  
  *說明*：若瀏覽器沒有自動開啟，請手動在瀏覽器上輸入以下網址：  
  `http://localhost:5173/<專案名稱>/pages/index.html`

- `npm run build`  
  編譯專案以進行正式部署，該模式不會自動開啟瀏覽器。

- `npm run deploy`  
  進行自動化部署，將專案部署至 GitHub Pages。

## 資料夾結構
├── assets # 靜態資源放置處 │ ├── images # 圖片放置處 │ └── scss # SCSS 樣式放置處 ├── layout # EJS 模板放置處 ├── pages # 頁面放置處 └── main.js # JavaScript 程式碼


- JavaScript 程式碼可寫在 `main.js` 檔案中。

### 注意事項
- `index.html` 是預設首頁，請不要隨意更改檔案名稱。
- `.gitignore` 檔案會忽略掉不應上傳至 GitHub 的檔案（例如 `node_modules`），請不要移除此檔案。

## 開發模式的監聽
當您啟動 `npm run dev` 後，Vite 會自動開始監聽檔案變動，無需手動使用 `Live Sass Compiler` 的 `Watch SCSS` 功能。

## 部署 gh-pages 流程說明

### Windows 版本
1. **在 GitHub 建立一個新的 Repository**  
   前往 GitHub 創建一個新的儲存庫。

2. **初始化 Git 儲存庫並推送原始碼**  
   在專案根目錄下開啟終端機並執行以下指令：
   ```bash
   git init            # 若已初始化過可跳過
   git add .           # 加入檔案至 Git 暫存區
   git commit -m "first commit"  # 提交第一次變更
   git branch -M main  # 設定為主要分支
   git remote add origin [GitHub Repository URL]  # 輸入 GitHub 儲存庫的 URL
   git push -u origin main  # 推送原始碼至 GitHub

執行自動部署
上傳原始碼後，執行 npm run deploy 進行自動化部署。這會將專案推送到 GitHub Pages。

 
