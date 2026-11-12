# n8n 教學投影片課程地圖

建議以「收到訂單並整理資料」為主線。先讓學員看懂一個流程如何啟動，再比較向外查詢與被外部觸發，最後介紹 Codex 如何透過 MCP 連到 n8n。

| 順序 | 學習成果 | 投影片或講師示範 | 引用頁 |
| --- | --- | --- | --- |
| 1 | 能在畫布指出觸發節點、處理節點與輸出 | 手動啟動後整理一筆虛構訂單，在執行紀錄查看結果 | [工作流程基礎](concepts/workflow-basics.md) |
| 2 | 能從 API 文件找出方法、端點和參數 | 用 GET 向模擬訂單 API 查詢，標出 HTTP 請求和回應 | [API 與 HTTP](concepts/api-http.md) |
| 3 | 能區分 Test URL 與 Production URL | 模擬外部系統 POST 訂單，觀察 Webhook 收到的 JSON | [Webhook](concepts/webhook.md) |
| 4 | 能把重複工作拆成輸入、判斷與輸出 | 以表單歸檔和訂單分流比較流程複雜度 | [自動化案例與選題](concepts/automation-cases.md) |
| 5 | 能用 AI 分類結果決定流程分支 | 用合成郵件示範詢價回信草稿與人工處理通知 | [AI 郵件分類](concepts/ai-email-routing.md) |
| 6（延伸） | 能指出 MCP 用戶端、伺服器與授權範圍 | 畫出 Codex CLI 連接 n8n 的路徑，說明 OAuth 授權 | [Codex MCP](concepts/codex-mcp.md) |

## 備課時如何引用

每頁投影片保留一個學習重點。在講者備註附上 Wiki 概念頁、該頁引用的原始網址，以及適用版本或查閱日期。流程圖與虛構訂單是教學設計。畫面、節點參數及預期輸出需以選定版本驗證後更新。

可先在 [Wiki 索引](index.md) 閱讀五篇完整來源筆記，再使用主題頁備課。
