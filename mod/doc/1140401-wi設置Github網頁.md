# 1. 緣起目的

## 緣起

配合建置簡單網站需求，需快速建立符合基本業務規則及技術架構的展示平台。

## 目的

本文件說明如何設置一個簡單的 Github 網站，涵蓋從環境設定、檔案架構建立，到最終測試之全流程。

# 2. 背景資訊

## 適用環境

### 網頁結構

本做法適用標準 HTML5 檔案（含 JavaScript），能在主流瀏覽器中正常運作。  

## Github Page功能

Github Pages 是 Github 提供的靜態網站託管服務，可直接從指定的 Repository 部署網站。  
* 利用 Repository 中的檔案（如 index.html）生成網站。  
* 支援自訂網域名稱。  
* 適用於個人或專案展示網站。  

# 3. 內容程序

## 設置Github組態

以下步驟將指引您完成 Github Pages 的基本設置：  

1. **建立 Repository**  
   - 登入 Github，點選「New Repository」，輸入 Repository 名稱與描述。  
   - 選擇是否初始化 README 文件。  

2. **設定 Repository 分支與目錄結構**  
   - 網站檔案只能放置於 Repository 的 (1)`根目錄`或 (2)`docs` 目錄中。  

3. **啟用 Github Pages 功能**  
   - 進入 Repository 的「Settings」頁面，找到「Pages」設定。  
   - 選擇來源分支（如 main 分支）及資料夾（根目錄或 `docs`），然後儲存設定。  
   - Github 將生成一個網址（通常為 `https://<username>.github.io/<repository>/`）供預覽網站。 

## 準備網站(頁)檔案

請依下列步驟準備並上傳您的網頁檔案：  

1. **準備網頁檔案**  
   - 編寫 HTML、CSS 與 JavaScript 檔案。  
   - 確保各檔案間的連結（如 CSS、JS）正確無誤。  
   - 可參考下方範例：
     
     ```html
     <!-- index.html -->
     <!DOCTYPE html>
     <html lang="zh-Hant">
     <head>
         <meta charset="UTF-8">
         <meta name="viewport" content="width=device-width, initial-scale=1.0">
         <title>簡單Github網站</title>
         <!-- 載入 CSS 樣式 -->
         <link rel="stylesheet" href="styles.css">
     </head>
     <body>
         <!-- 主內容區域 -->
         <header>
             <h1>歡迎光臨</h1>
         </header>
         <main>
             <p>這是一個示範網站，使用 Github Pages 部署。</p>
         </main>
         <footer>
             <p>聯絡資訊：example@example.com</p>
         </footer>
         <!-- 載入 JavaScript 程式碼 -->
         <script src="script.js"></script>
     </body>
     </html>
     ```

## 測試

請依下列步驟檢查網站是否正常運作：  

1. **上傳後預覽**  
   - 完成所有檔案上傳後，進入 Repository 的「Settings」 -> 「Pages」確認生成的預覽網址。  
   - 點選網址，檢查網站首頁是否正確顯示。  
   <!-- GPTHELP：提示如何找到並使用預覽網址 -->

2. **檢查各頁面與連結**  
   - 點擊網站內的連結，確保所有頁面均能正確導向與顯示。  
   - 檢查是否有 JavaScript 錯誤或 CSS 載入問題。  
   <!-- GPTHELP：說明測試過程中常見問題與解決辦法 -->

3. **調整與重上傳**  
   - 若發現問題，根據瀏覽器控制台或錯誤訊息調整程式碼。  
   - 重新上傳更新檔案，並再次測試。  
   <!-- GPTHELP：確保步驟詳盡，便於使用者追蹤問題 -->

# 4. 結論備註

本文件提供了一個簡單 Github 網站設置的完整流程說明。  
使用者可依據上述步驟，從 Repository 建立、檔案上傳到最終測試，完成一個基本展示網站的部署。  
未來可依需求進行功能擴充與設計優化。
