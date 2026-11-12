---
title: "Codex CLI 與 n8n MCP"
type: concept
tags: ["n8n","codex-mcp"]
sources: ["sources/n8n-codex-mcp.md"]
last_updated: 2026-11-13
status: reviewed
---

# Codex CLI 與 n8n MCP

## 核心概念

MCP 讓支援的用戶端發現與呼叫伺服器提供的工具。此案例的用戶端是 Codex CLI，伺服器由 n8n 實例提供。工具與工作流程的可用範圍取決於實例設定、帳號授權與工作流程的存取設定。

## 投影片可用的操作順序

1. 在 n8n 實例設定啟用 Instance-level MCP，從連線介面複製 Server URL。
2. 使用官方文件的 Codex CLI OAuth 設定。完成伺服器登錄後，使用 `codex mcp login n8n` 進行授權。
3. 在測試實例確認可見的工具和工作流程，記錄結果。若認證失敗，先確認完整端點、授權狀態及版本。

可用一張圖標出「Codex CLI → n8n MCP Server → 已授權的工作流程」。正式錄製前應確認 CLI 與 n8n 版本、端點和實際畫面。本次為文件整理，未建立連線。

來源：[n8n 官方 Codex CLI 連線章節](../sources/n8n-codex-mcp.md)。
