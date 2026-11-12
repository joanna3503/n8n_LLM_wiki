---
title: "Slow Signals：第一個 AI 郵件工作流程"
type: source
tags: [n8n]
sources: []
last_updated: 2026-11-13
status: reviewed
---

# Slow Signals：第一個 AI 郵件工作流程

## 情境與環境
Slow Signals 於 2026-06-04 發表，06-07 更新。案例處理新信分類、初步回覆和人員通知。文章比較 Cloud、Docker 自架與 npx，實作依賴 Gmail、Anthropic 和 Slack 的連線或憑證。

## 郵件分流
1. Gmail Trigger 收到新信後提供郵件資料。
2. AI Agent 搭配 Anthropic Chat Model，將郵件判定為詢價、合作、垃圾信或需本人處理。分類輸出用固定值供後續節點判斷。
3. IF 根據分類結果分流。詢價分支可用固定回覆模板加上模型調整，交給 Gmail Reply。
4. 需本人處理的分支用 Slack 提醒，附寄件人、主旨與摘要。原文未細寫其餘兩類的動作。

## 教材釐清
分類與草擬回信是兩個輸出任務。示範可先用合成郵件檢查分類、回信草稿與未預期結果。模型按量計費，送交雲端模型的郵件內容會離開自架環境。若另用公開 Webhook，須設計認證。

## 原文

[閱讀來源](https://vocus.cc/article/6a1be5b5fd897800016df01b) · 查閱日期 2026-11-13
