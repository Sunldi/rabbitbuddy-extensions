# rabbitbuddy-extension
RabbitBuddy插件市场
# RabbitBuddy 插件市场（货架清单）

这份仓只放两样东西：`index.json`（货架）与 `icons/`（图标）。
**插件包体不放这里**——放到你自己仓库的 GitHub Releases，把绝对下载地址写进 index.json。

## 上架 / 更新：提 PR 改 index.json

一条 = 一个可安装的版本。必填五格：`id` / `displayName` / `description` / `version` / `downloadUrl`。

```json
{
  "schema": "rb.ext.market/v1",
  "extensions": [
    {
      "id": "sheet-studio",
      "displayName": "表格工坊",
      "description": "在侧栏里清洗与透视本地 CSV",
      "version": "1.2.0",
      "category": "data",
      "downloadUrl": "https://github.com/<你>/<仓>/releases/download/v1.2.0/sheet-studio.zip",
      "sha256": "<zip 的 64 位十六进制 sha256>",
      "sizeBytes": 81234,
      "icon": "icons/sheet-studio.png",
      "publishedAt": "2026-11-06",
      "author": "<作者>",
      "homepage": "https://github.com/<你>/<仓>",
      "featured": false,
      "tags": ["Excel", "表格"]
    }
  ]
}
