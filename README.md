# Node.js Survey Response Handler

## 簡介
這個專案是一個簡單的 Node.js 函數，用於處理來自用戶的調查輸入。用戶需輸入一個特定的通關密語，以便確認其有效性。該函數可作為 AWS Lambda 函數或類似伺服器無關的計算平台上運行。

## 功能
- 驗證用戶輸入的通關密語。
- 返回相應的 HTTP 狀態碼以及提示訊息。
- 支援 CORS 設定，允許來自不同來源的請求。

## 安裝與使用方式
1. 確保您的系統已安裝 Node.js 環境（推薦版本 14.x 或以上）。
2. 將程式碼複製到`.js`檔案中（例如：`handler.js`）。
3. 在伺服器或雲服務上設置該函數，例如使用 AWS Lambda。
4. 利用 POST 請求調用該函數，並在請求主體中包含一個JSON格式的 `value` 屬性，例如：
   ```json
   {
       "value": "cake"
   }
   ```

## 必要的依賴模組清單
此專案無需額外依賴模組，僅使用 Node.js 內建功能。

## 授權條款
本專案使用 MIT 授權條款，您可以自由使用及修改此程式碼，但不承擔任何責任。請參閱 `LICENSE` 檔案以了解更多相關資訊。

---

隨時歡迎提交問題或功能需求，以幫助我們改進此函數！