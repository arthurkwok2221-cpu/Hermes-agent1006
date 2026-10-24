# Hermes-agent1006

Arthur Kwok 的 Web 專案導覽與前端應用，部署於 GitHub Pages。

## 專案結構

| 路徑 | 說明 |
|---|---|
| `index.html` | Navigator 導覽頁（卡片、搜尋、分類篩選） |
| `projects.json` | 專案清單資料源 — 新增專案只改此檔 |
| `todolist/` | TodoList 應用 |
| `dashboard/` | 銷售儀表板（Dashboard_Data.xlsx） |
| `slides/` | 會議簡報（AI 課程與 OpenClaw） |

## 新增專案

1. 在 `projects.json` 的 `projects` 陣列加入一筆：`name / description / stack / category / status / url`。
   - `status`：`已上線` 或 `開發中`
   - `url`：相對路徑（例如 `myapp/`）或外部連結
2. 若是新 app，把 HTML 放到對應子資料夾（如 `myapp/index.html`）。
3. 推送至 `main`，CI（`.github/workflows/deploy-pages.yml`）自動重新部署。

## 部署

`.github/workflows/deploy-pages.yml`：push 至 `main` 時上傳整個根目錄到 Pages。
公開網址：https://arthurkwok2221-cpu.github.io/Hermes-agent1006/
