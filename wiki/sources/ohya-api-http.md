---
title: "好事發生數位的 API 與 HTTP 案例"
type: source
tags: [n8n]
sources: []
last_updated: 2026-11-13
status: reviewed
---

# 好事發生數位的 API 與 HTTP 案例

## API 與 HTTP
API 約定軟體能呼叫哪些操作。HTTP 定義請求和回應的交換方式。GET 常用於讀取，POST 用於提交，PUT 常見於替換，PATCH 用於部分更新，DELETE 用於刪除。HEAD 可查閱回應標頭，OPTIONS 可詢問通訊選項。具體效果依端點規格。

## GPT Actions 串接案例
1. 在 n8n 新增 Webhook，指定 POST 與路徑。
2. 在自訂 GPT 的 Action 中用 OpenAPI 描述伺服器、路徑、操作識別字及 JSON 欄位。文章案例要求 `message`，並允許附上 `userId`。
3. 先使用 Test URL 並讓 n8n 監聽。用自然語言觸發 Action，在 Webhook 輸出確認收到的內容。
4. 上線時核對發佈狀態、正式 URL 與認證，再用正式設定驗證。

## 教材釐清
以文章的 OpenAPI 範例為準，Action 是發出 POST 的呼叫端，n8n 是接收端。HTTP 回應由 n8n 返回呼叫端。原文部分段落混用了回呼說法，授課圖應標清兩個方向。

## 原文

[閱讀來源](https://cms.ohya.co/n8n-ai-automation/what-is-api-http/) · 查閱日期 2026-11-13
