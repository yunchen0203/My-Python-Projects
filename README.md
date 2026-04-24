# My-Python-Projects
這是一個存放 Python 練習與開發紀錄的儲存庫。

## 🛠️ 目前專案內容

### ✒️ QuickSign.ipynb (重點專案)
* **功能描述**: 為了解決傳統紙本簽到效率低、易出錯問題而開發的自動化簽名處理工具。
* **語言**: Python 3
* **主要函式庫**: `pandas`, `openpyxl`
* **開發環境**: Jupyter Notebook / VS Code
* **進度**: 開發中
  
#### 🌟 核心功能
1. **自動化名單導入**：利用 `pandas` 串接 `.xlsx/csv` 檔案，實現學生資訊自動初始化，取代人工錄入。

2. **重複簽到攔截**：透過邏輯判斷實作即時檢核，防止重複輸入同一學號，確保簽到數據的唯一性與信賴度。

3. **健全的異常處理**：內建 `try-except` 與格式檢核（如長度限制、類型檢查），能有效過濾輸入錯誤，維持系統穩定運行。

4. **格式化資料匯出**：整合 `openpyxl` 引擎，匯出前自動執行「班級座號排序」，產出可直接使用的標準化 Excel 報表。

* **詳細描述**：簽到結束後，程式會自動依照「班級」或「學號」進行升冪排序，並生成帶有當前時間戳記（Timestamp）的新報表。這解決了傳統紙本簽到後，還需要人工二次輸入與排序的痛點。

#### 🧠 使用的程式邏輯
* **迴圈 (Loops)**: 用於逐行檢查名單資料與持續等待輸入。
* **條件判斷 (If-Else)**: 判斷學號是否存在於名單中。
* **例外處理 (Try-Except)**: 防止輸入錯誤導致程式中斷。

#### 📐 流程圖
<img width="6108" height="3920" alt="messageImage_1776926951694" src="https://github.com/user-attachments/assets/b4b54e70-fa8e-4092-a2b3-f337a45a0868" />

---

### 🧪 main.py (測試檔案)
* 此檔案為初始環境測試檔案（目前為空值，僅用於確認 GitHub 上傳流程）。

---

## 🚀 如何開始

1. **環境需求**: 建議安裝 [Anaconda](https://www.anaconda.com/) 或 [VS Code](https://code.visualstudio.com/) 並搭配 Jupyter Extension。
2. **運行方式**: 開啟 `QuickSign.ipynb` 後，點擊「Run All」或依序執行單元格。

## 📈 學習目標
* [ ] 完善 QuickSign 的功能介面。
* [ ] 新增更多自動化腳本。
* [ ] 練習撰寫更規範的 Python 代碼。
