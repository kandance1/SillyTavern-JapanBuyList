# 日本購物清單（SillyTavern 擴充）

拍商品照片 → 自動辨識 → 用 BigGo 查台灣／日本價格 → 換算台幣價格區間。勾「已買」就移到已買。另有「用 Gemini 查詢商品研究」（功用、規格、優缺點）。

## 安裝
**方法 A（一鍵安裝）：** 酒館 →「擴充功能」→「安裝擴充功能」→ 貼上 `https://github.com/kandance1/SillyTavern-JapanBuyList` → 安裝。

**方法 B（手動）：**
1. 把整個 `japan-buy-list` 資料夾放進 SillyTavern 的使用者擴充目錄：
   `SillyTavern/data/default-user/extensions/japan-buy-list/`
2. 重新整理酒館網頁（Cmd/Ctrl+Shift+R）。
3. 打開：輸入框旁的魔術棒選單 →「日本購物清單」，或「擴充功能」設定頁裡的「日本購物清單」→「開啟購物清單」。

## 更新
酒館 →「擴充功能」→「管理擴充功能」→ 找到「日本購物清單」按更新，再重新整理網頁。

## 使用前要設定（每個人用自己的）
- 辨識照片需要你自己的 Google AI Studio 金鑰：
  酒館上方插頭圖示（API 連線）→ Chat Completion → Google AI Studio → 貼上你自己的金鑰 → Connect。
  金鑰取得：aistudio.google.com/apikey（免費金鑰即可辨識照片）。
- 查價用 BigGo，不需要金鑰。

## 資料與隱私
- 商品與照片只存在你使用的那個瀏覽器（IndexedDB），不會上傳到任何伺服器。
- 辨識照片時，圖片會暫時傳給 Google AI。
- 換瀏覽器或清除網站資料會消失，請定期「匯出清單」。匯出檔可匯入網頁版，反之亦然。

## 新增照片
按「新增商品照片」，或把照片拖進視窗，或按 Cmd/Ctrl+V 貼上圖片。
