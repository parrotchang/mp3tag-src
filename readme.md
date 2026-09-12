# Mp3tag Web Source Script for Apple Music

這是一個專為 [Mp3tag](https://www.mp3tag.de/) 設計的 Web Source 腳本（Tag Source）。它可以幫助您直接從 Apple Music 的資料庫中獲取音樂資訊，並自動寫入音訊檔案的 ID3 v1 或 ID3 v2 標籤中。

## ✨ 功能特色 (Features)

* **精準獲取標籤**：從 Apple Music 抓取最準確的官方音樂資訊，支援寫入 ID3 v1 與 ID3 v2 格式。

* **完整中繼資料**：自動填入包含歌曲名稱、演出者 (Artist)、專輯 (Album)、發行年份 (Year)、音樂類型 (Genre)、音軌編號 (Track Number) 等資訊。

* **高畫質專輯封面**：支援直接下載並嵌入 Apple Music 的高解析度專輯封面圖片。

* **操作簡便**：無縫整合至 Mp3tag 的標籤來源選單中。

## 📥 安裝步驟 (Installation)

1. 下載本專案的壓縮檔，並將其解壓縮 (Windows 請使用 7-zip 解壓縮)。

2. 找到解壓縮後的腳本檔案（副檔名通常為 `.src` 或是 `.inc`）。

3. 開啟 Mp3tag 軟體。

4. 點擊頂部選單的 **「檔案 (File)」** -> **「開啟設定資料夾 (Open configuration folder)」**。

   * *提示：您也可以直接按下快捷鍵 `Ctrl + Q`，或是在檔案總管前往 `%appdata%\Mp3tag\`*

5. 進入 `data\sources` 資料夾。

6. 如果您使用的是 Mac 版本的 Mp3tag，請將檔案放入以下路徑：

   ~/Library/Containers/app.mp3tag.Mp3tag/Data/Library/Application Support/Mp3tag/data/sources

  **Mac 使用者快速開啟提示：
由於 Mac 的系統資料夾較深，最快的開啟方式是啟動 Mp3tag 應用程式，點選左上角選單列的 Mp3tag -> Preferences... (偏好設定) -> 切換到 Sources (標籤來源) 頁籤，接著點擊下方的 Open sources folder 按鈕，即可直接開啟該資料夾並將檔案放進去。**

8. 將剛剛解壓縮出來包含腳本在內的三種檔案`.src`, `.ini`, `settings`複製到這個 `sources` 資料夾內。

9. 重新啟動 Mp3tag 以載入腳本。

## 🚀 使用說明 (Usage)

1. 將您需要修改標籤的音樂檔案拖曳到 Mp3tag 軟體視窗中。

2. 選取您想要更新標籤的檔案（可按 `Ctrl + A` 全選）。

3. 點擊頂部選單的 **「標籤來源 (Tag Sources)」**。

4. 在下拉選單中找到並點擊 **「Apple Music」**（或是您為該腳本自訂的名稱）。

5. 系統會彈出搜尋視窗，請輸入**專輯名稱**或**歌手名稱**進行搜尋。

6. 從搜尋結果中選擇正確的專輯。

7. 確認左側抓取的資料與右側您的檔案對應無誤後，點擊 **「確定 (OK)」** 即可將 Apple Music 的 ID3 標籤與封面寫入您的檔案中。

## ⚠️ 注意事項 (Notes)

* 本腳本需在網路連線正常的情況下使用。

* Apple Music 的搜尋結果可能會因地區 (Region) 設定而有所不同，如有需要，可自行在 `.src` 原始碼中修改 API 請求的地區代碼（如 `tw`、`us`、`jp` 等）。

* 本腳本僅供個人整理音樂庫使用，請勿用於任何商業用途。

## 🤝 貢獻與回饋 (Contributing)

如果您在使用過程中遇到任何問題，或是發現腳本因為 Apple Music 網頁結構改變而失效，歡迎提交 [Issue](https://github.com/) 或發起 Pull Request 協助修復！
