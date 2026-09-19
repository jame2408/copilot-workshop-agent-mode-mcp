![工作坊完成徽章](https://img.shields.io/badge/GitHub_Copilot_實戰工作坊-已完成-1F883D?style=for-the-badge&logo=githubcopilot&logoColor=white)

# 待辦清單 Web App

這是一個在 GitHub Copilot 實戰工作坊中完成的待辦清單 Web App。專案以純前端技術實作，提供日常待辦事項的新增、整理與狀態管理功能，並支援淺色與深色主題切換。

## 線上展示

GitHub Pages：<https://jameswang.pro/copilot-workshop-agent-mode-mcp/>

## 功能

- 新增待辦事項，空白內容不會被加入。
- 勾選或取消勾選待辦事項，完成項目會顯示刪除線並淡化。
- 刪除單筆待辦事項。
- 清除所有已完成的待辦事項。
- 顯示整體未完成待辦事項數量。
- 依「全部」、「未完成」與「已完成」篩選清單。
- 篩選結果為空時顯示對應提示文字。
- 在淺色模式與深色模式之間切換。
- 使用者手動選擇的主題會保存，重新整理後仍然維持。
- 沒有手動主題偏好時，依照作業系統的深淺色設定顯示。
- 使用 `localStorage` 保存待辦事項資料。
- 支援手機螢幕與響應式版面。

## 技術

- 使用純 HTML、CSS 與原生 JavaScript。
- 不使用任何前端框架或套件，也不依賴外部 CDN。
- 使用 CSS 變數集中管理淺色與深色主題的配色。
- 使用 `localStorage` 保存待辦資料與主題偏好。
- 使用原生 DOM API 建立清單內容。

## 開發方式

- 使用 GitHub Copilot Agent Mode，依照需求建立與修改前端檔案，並在每次變更後進行檢查與瀏覽器驗證。
- 使用 MCP 連接 Microsoft Learn 文件，查詢 `prefers-color-scheme` 與深色模式色彩對比等官方建議。
- 使用 GitHub MCP 讀取 issue、建立修正分支、推送變更並建立 Pull Request。
- 在 `.github/prompts/fix-issue.prompt.md` 定義 agentic workflow，規範從讀取 issue、提出計畫、修改與驗證，到提交、推送及建立 Pull Request 的流程。

## 我學到什麼

- 了解如何使用 Agent Mode 讓 AI 根據完整需求直接建立與修改多個專案檔案。
- 練習使用 `localStorage` 保存瀏覽器端資料，讓重新整理後的使用者狀態仍然存在。
- 了解如何用 CSS 變數與 `prefers-color-scheme` 實作可切換且能跟隨系統設定的主題。
- 練習透過 MCP 讀取 Microsoft Learn 與 GitHub 的外部資訊，將文件與 issue 納入開發流程。
- 學會用 `.github/prompts` 把重複的 issue 修正流程整理成可重複執行的 agentic workflow。
