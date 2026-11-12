---
title: "API、HTTP 與 HTTP Request"
type: concept
tags: ["n8n","api-http"]
sources: ["sources/ohya-api-http.md","sources/n8n-http-request.md"]
last_updated: 2026-11-13
status: reviewed
---

# API、HTTP 與 HTTP Request

## 核心概念

API 定義可呼叫的操作和資料規格。HTTP API 以請求與回應交換資料。讀 API 文件時先找出方法、端點、認證、請求欄位與回應格式，再對照到節點設定。

| 元素 | 問題 | 示意值 |
| --- | --- | --- |
| Method | 呼叫什麼操作？ | GET |
| URL | 呼叫哪個端點？ | `https://api.example.test/orders` |
| Query | 如何篩選？ | `status=pending` |
| Headers | 有哪些中繼資料？ | `Accept: application/json` |
| Body | 要送哪些資料？ | 依端點文件填寫 |
| Response | 如何知道結果？ | 狀態碼與回應內容 |

GET 常用於讀取，POST 可用來建立資料或提交操作，PUT 常用於替換，PATCH 常用於部分更新，DELETE 常用於刪除。每個端點的參數與實際效果以其文件為準。

## 投影片與示範

畫出 n8n 的 HTTP Request 節點向模擬訂單 API 送出 GET，API 回傳一筆訂單。讓學員將方法、URL、篩選條件分別填到節點欄位，並比較成功回應與路徑輸入錯誤時的結果。表中的 URL 為示意。

來源：[好事發生數位](../sources/ohya-api-http.md)、[n8n 官方文件](../sources/n8n-http-request.md)。延伸：[Webhook](webhook.md)。
