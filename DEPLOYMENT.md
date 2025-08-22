# 🚀 GitHub Pages 部署指南

這份指南將幫助你將 C# 學習網站部署到 GitHub Pages，讓全世界都能訪問你的學習資源！

## 📋 部署前準備

### 需要的工具
- GitHub 帳號（免費）
- 現代瀏覽器
- （可選）Git 軟體

### 檔案清單
確保你有以下檔案：
- `index.html` - 主要的學習網站
- `README.md` - 專案說明
- `DEPLOYMENT.md` - 這個部署指南

## 🎯 快速部署（5 分鐘完成）

### 步驟 1：建立 GitHub 倉庫

1. 前往 [GitHub.com](https://github.com)
2. 點擊右上角 **"+"** → **"New repository"**
3. 設定倉庫：
   - Repository name: `csharp-learning-guide`
   - Description: `完整的 C# 學習指南 - 互動式網頁教學`
   - 選擇 **Public**（必須是公開才能使用 GitHub Pages）
   - 勾選 **"Add a README file"**
4. 點擊 **"Create repository"**

### 步驟 2：上傳檔案

1. 在新建的倉庫頁面，點擊 **"uploading an existing file"**
2. 將所有檔案拖曳到上傳區域：
   - `index.html`
   - `README.md`
   - `DEPLOYMENT.md`
3. 在下方 "Commit changes" 區塊：
   - Commit message: `初始化 C# 學習網站`
   - Description: `新增完整的互動式 C# 學習指南`
4. 點擊 **"Commit changes"**

### 步驟 3：啟用 GitHub Pages

1. 在倉庫頁面，點擊 **"Settings"** 頁籤
2. 在左側選單向下捲動，找到 **"Pages"**
3. 在 "Source" 區塊：
   - 選擇 **"Deploy from a branch"**
   - Branch: 選擇 **"main"**
   - Folder: 選擇 **"/ (root)"**
4. 點擊 **"Save"**

### 步驟 4：等待部署完成

1. GitHub 會顯示一個綠色橫幅說明網站正在建置
2. 通常需要 2-5 分鐘完成
3. 完成後會顯示你的網站網址：`https://你的用戶名.github.io/csharp-learning-guide`

## 🔧 進階部署選項

### 使用 Git 命令列部署

如果你熟悉命令列操作：

```bash
# 1. 複製倉庫到本地
git clone https://github.com/你的用戶名/csharp-learning-guide.git

# 2. 進入專案目錄
cd csharp-learning-guide

# 3. 複製所有檔案到這個目錄

# 4. 添加檔案
git add .

# 5. 提交變更
git commit -m "新增 C# 互動式學習網站"

# 6. 推送到 GitHub
git push origin main
```

### 自定義網域名稱（進階）

如果你有自己的網域名稱：

1. 在倉庫根目錄建立 `CNAME` 檔案
2. 檔案內容只需要一行：`你的網域名稱.com`
3. 在你的網域 DNS 設定中加入 CNAME 記錄指向 `你的用戶名.github.io`

## 📱 測試你的網站

### 桌面測試
1. 開啟你的網站網址
2. 測試所有互動功能：
   - 點擊課程標題展開內容
   - 使用互動練習輸入數值
   - 點擊解答按鈕查看答案
3. 檢查響應式設計：調整瀏覽器視窗大小

### 手機測試
1. 用手機開啟網站
2. 確認文字大小適中
3. 測試觸控操作
4. 檢查橫向和直向顯示

## 🚀 網站效能優化

### 載入速度優化
- 所有外部資源（字體、CSS、JavaScript）都使用 CDN
- 圖片使用 Emoji，無需額外載入
- CSS 和 JavaScript 已經過優化

### SEO 優化
網站已包含：
- 適當的 meta 標籤
- 語意化 HTML 結構
- 響應式設計
- 無障礙設計考量

## 🔄 更新網站內容

### 方法 1：GitHub 網頁編輯
1. 在 GitHub 倉庫中點擊要編輯的檔案
2. 點擊鉛筆圖示 **"Edit this file"**
3. 進行修改
4. 填寫 commit 訊息
5. 點擊 **"Commit changes"**

### 方法 2：重新上傳
1. 修改本地檔案
2. 在 GitHub 倉庫中刪除舊檔案
3. 上傳新檔案

### 方法 3：Git 推送
```bash
# 修改檔案後
git add .
git commit -m "更新學習內容"
git push origin main
```

## 📊 監控與分析

### GitHub Pages 狀態
- 在倉庫的 "Settings" → "Pages" 可以看到部署狀態
- 在 "Actions" 頁籤可以看到建置歷史

### 訪客統計（可選）
可以添加免費的網站分析服務：
- Google Analytics
- GitHub 提供的基本統計

## 🆘 常見問題解決

### 問題：網站顯示 404 錯誤
**解決方案：**
- 確認 GitHub Pages 已啟用
- 檢查檔案名稱是否為 `index.html`
- 等待 5-10 分鐘讓變更生效

### 問題：樣式沒有載入
**解決方案：**
- 檢查網路連線
- 確認 CDN 連結是否正確
- 清除瀏覽器快取

### 問題：互動功能無效
**解決方案：**
- 檢查 JavaScript 是否被瀏覽器封鎖
- 確認檔案完整上傳
- 檢查瀏覽器開發者工具的錯誤訊息

### 問題：手機顯示異常
**解決方案：**
- 確認 viewport meta 標籤存在
- 檢查 CSS 的響應式設計
- 測試不同瀏覽器

## 📈 進階功能

### 添加留言功能
可以使用以下免費服務：
- Disqus
- Utterances（使用 GitHub Issues）

### 添加搜尋功能
- 使用 Lunr.js 實作客戶端搜尋
- 或整合 Google 自訂搜尋

### 多語言支援
- 建立不同的 HTML 檔案
- 使用 JavaScript 切換語言

## 🎉 部署完成！

恭喜你！現在你有了一個專業的 C# 學習網站。

### 分享你的網站
- 複製網址分享給朋友
- 在社群媒體上分享
- 提交到程式學習資源列表

### 持續改進
- 收集使用者回饋
- 定期更新學習內容
- 添加新的互動功能

---

**祝你部署順利！如果遇到問題，歡迎在 GitHub Issues 中詢問。** 🚀
