---
title: "雷蒙的 n8n 入門指南"
type: source
tags: [n8n]
sources: []
last_updated: 2026-11-13
status: reviewed
---

# 雷蒙的 n8n 入門指南

## 介面與流程
侯智薰（雷蒙）於 2025-04-03 發表，頁面標示 2026-10-20 更新。畫布用來連接節點，Credentials 管理憑證，Executions 提供逐次執行的結果與除錯線索。設計流程時先定義觸發條件、後續操作和資料去向。

## 節點速查
| 節點 | 用途 |
| --- | --- |
| Manual Trigger | 由操作者手動開始，適合逐步試跑 |
| Webhook | 接收外部事件，例如訂單通知 |
| Schedule Trigger | 按時執行，例如每週產出報表 |
| Loop Over Items | 控制逐批處理，例如分批寄通知 |
| Edit Fields (Set) | 改欄位名稱、增欄位或統一資料格式 |
| If | 依條件選擇兩條執行路徑 |
| Code | 內建節點不足時補上自訂資料處理 |

## 選題與維護
優先找重複、耗時而且規則清楚的工作。可拆解既有模板理解設計，再用測試資料逐節點驗證。把設計原因和步驟寫在 Sticky Notes，方便日後排錯。原文畫面和部署資訊有版本背景，備課時應以授課環境核對。

## 原文

[閱讀來源](https://raymondhouch.com/lifehacker/digital-workflow/n8n-beginner-guide/) · 查閱日期 2026-11-13
