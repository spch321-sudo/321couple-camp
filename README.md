# 321couple-camp

## v24-up1103（2026-11-03）自動更新（確認版）
- 原本 `sw.js` 為快取優先、改版全靠手動升快取號，且清快取時會刪光同網域所有 App 的快取。已改為正規自動更新：網路優先（HTML／JS／JSON）、只清自己前綴（`cc321-`、舊 `couples-321-v23`）的快取。
- 加入通用自動更新掛件 `upd321.js`：`version.json` 輪詢＋`reg.update()`，空閒時自動換新版，輸入中／朗讀中只顯示頂端更新條，結束後自動套用；防無限重整。「我們」頁新增「版本與更新」（檢查更新／強制更新）。`index.html` 與 `繁體index.html` 都已加入。
- 版本 `v24-up1103` 四處一致：`version.json`、`sw.js`、`index.html`／`繁體index.html`（APPVER）、本 README。
- 註：本 repo 為夫妻成長營早期版本（現行為三語的 321couples），仍補上自動更新，避免已安裝的使用者卡在舊版。

