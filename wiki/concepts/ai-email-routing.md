---
title: "AI 郵件分類與分流"
type: concept
tags: [n8n]
sources: ["sources/slow-signals-ai-workflow.md", "sources/arthlai-n8n-cases.md"]
last_updated: 2026-11-13
status: reviewed
---

# AI 郵件分類與分流

## 工作流程設計

Gmail Trigger 提供郵件，模型從可預期的類別中選一個，IF 依固定值分流。詢價可以產生回信草稿，需本人處理則輸出摘要通知。這個架構也能套用到客服案件或表單分派。

| 測試輸入 | 應觀察的結果 |
| --- | --- |
| 詢問服務價格 | 分到詢價，產生待確認的回信草稿 |
| 需要個人判斷的來信 | 分到人工處理，輸出主旨和摘要 |
| 空白、模糊或分類不在預期內 | 進入人工檢查，保留原始輸入供排查 |

## 教學示範

先在 n8n 用固定的合成郵件測試，將兩個分支的輸出顯示在節點結果。先驗證分類值、欄位對應與例外，再示範如何接 Gmail Reply 或 Slack。回信草稿另設生成步驟，便於獨立檢查。上述測試表為課堂設計，尚待實測。

來源筆記：[第一個 AI 郵件工作流程](../sources/slow-signals-ai-workflow.md)、[自動化場景](../sources/arthlai-n8n-cases.md)。
