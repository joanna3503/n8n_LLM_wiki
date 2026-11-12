---
title: "n8n 官方文件：Codex CLI 連接 MCP"
type: source
tags: [n8n]
sources: []
last_updated: 2026-11-13
status: reviewed
---

# n8n 官方文件：Codex CLI 連接 MCP

## 前置條件
在 n8n 開啟實例層級 MCP 存取，並從連線介面複製完整 Server URL。它通常以 `/mcp-server/http` 結尾。協定與主機名稱以實例提供的值為準。

## OAuth 與 token
官方優先建議 OAuth。先用 `codex mcp add n8n --url "<SERVER_URL>"` 登錄伺服器，再執行 `codex mcp login n8n` 完成授權。也可在 Codex 的 `config.toml` 設定 MCP 伺服器。

若選 token 方式，在伺服器設定附上 Authorization Bearer 標頭，使用 n8n 為 MCP 產生的 token。教材只顯示佔位值。舊版 Codex 可能需要 `experimental_use_rmcp_client` 功能旗標，應依版本確認。

## 驗證目標
以測試實例確認 OAuth 能完成、用戶端可看到預期工具、工作流程已開放相應存取。設定與驗證順序來自文件，尚未實機連線。

## 原文

[閱讀來源](https://docs.n8n.io/connect/connect-to-n8n-mcp-server/mcp-client-examples#connecting-codex-cli-to-n8n-mcp-server) · 查閱日期 2026-11-13
