# M480 Secure Boot ISP 更新指南

本機網頁投影片／操作指南，沿用 `/web` 既有 Nuvoton 頁面的側欄、字體、色彩及 Markdown／Mermaid 渲染方式。

- 可編輯原稿：`index.md`。
- 網頁入口：`index.html`。
- 網站路徑：`/slide_Nuvoton_secure_boot_operation_M480/`；知識庫首頁的 Nuvoton 平台專題提供入口。
- 共用版型：`../notices_can/assets/style.css`、`../notices_can/assets/app.js`；本專案未修改共用檔案。
- 網站圖片：`assets/screenshots/`；來源與處理方式見 `assets/screenshots/manifest.json`。
- 完整尺寸流程圖：`assets/diagrams/`；由原稿的三張 Mermaid 圖同步輸出。
- 本機驗證紀錄：`SELF_CHECK.md`。

## 內容範圍

ICP 的 Boot Loader／Security Lock、Secure Boot key 與 KPROM 配置；SecureBootTool 的 Waiting／Loading／認證、Key Options、首次兩區部署與後續 APROM-only 更新；以及自訂 LDROM、APROM／SRAM 的適用條件與限制。

已驗證專用 LDROM 流程與尚未實作的 SRAM 方案，在正文中分別標示。硬體結果來自使用者回報，網頁驗證不代表新增硬體測試。

## 本機預覽

在 `/web` 根目錄執行：

```powershell
python -m http.server 8768 --bind 127.0.0.1 --directory .
```

瀏覽 `http://127.0.0.1:8768/slide_Nuvoton_secure_boot_operation_M480/`。
由於入口會 fetch Markdown 並載入根路徑的共用資源，使用 HTTP 預覽，不以檔案總管直接開啟 HTML。
Markdown 與 Mermaid 使用與既有站點相同的固定版本 CDN，預覽需要能連線取得這些資源。

## 素材與資料範圍

`img/` 保留使用者原始素材，可能含個人路徑；`.gitignore` 排除此資料夾。頁面只引用 `assets/screenshots/` 的審閱版本。公開範例金鑰已獲使用者同意保留，供兩套工具輸入對照；個人路徑與識別資料需遮蔽。

圖片內的檔案大小、配置與 retry 參數為畫面示意，正式產品以其建置／部署紀錄為準。實際產品金鑰不收錄於一般診斷資料。

本次交付為本機專案與入口索引更新，尚未進行 Git push／部署。後續發布遵循 `/web/AGENTS.md` 與共用公開內容準則。
