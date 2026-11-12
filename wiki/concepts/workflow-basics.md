---
title: "工作流程、觸發與節點"
type: concept
tags: ["n8n","workflow-basics"]
sources: ["sources/raymond-n8n-beginner.md"]
last_updated: 2026-11-13
status: reviewed
---

# 工作流程、觸發與節點

## 核心概念

Workflow 由相連的節點組成。Trigger 決定啟動時機，後續節點可以整理資料、依條件分支或執行操作。一次執行的結果可以在 Executions 中追查。

| 啟動方式 | 適用情境 | 教學觀察點 |
| --- | --- | --- |
| 手動觸發 | 第一次練習與除錯 | 講師決定何時執行 |
| Schedule Trigger | 每天或每週的例行工作 | 交代排程時區 |
| Webhook | 外部系統傳來 HTTP 請求 | 核對 URL 和請求方法 |

## 投影片與示範

以一筆虛構訂單貫穿課程。先在畫布手動執行，建立 `orderId` 和 `amount` 欄位，再查看節點輸出。請學員指出觸發、處理與輸出各是哪一段。介面截圖在選定授課版本後拍攝。

來源：[雷蒙的 n8n 入門指南](../sources/raymond-n8n-beginner.md)。下一步：[API 與 HTTP](api-http.md)。
