# 321couple-camp

## v24-up1103-xz1103-xzm1103（2026-11-04）小智回答跟讀、畫線
- 小智的回答也能逐句跟讀（🔊）、點一下畫線、再點開面板（換色／領受／做成美圖／問小智／朗讀這句／從這裡朗讀／複製／分享／取消畫線）；畫線隨句子保存（`xzm_hl_couple-camp`），小智對話最近 60 則另存、重開 App 放回；「我們」頁小智設定卡之後新增「✨ 小智畫線」清單（原回答已不在對話中的畫線仍列出）。串流／出錯訊息與收合中的回答不切句。
- 通用外掛 `xzm.js`（preset.cc，朗讀接宿主 `xzSpeakAlong`）；`sw.js` 預快取加入 `./xzm.js`。
- 宿主只加兩個最小掛鉤（`繁體index.html`）：`window.__xzHost`（小智對話狀態）與 `window.__xzCard`（回答做成美圖）。`index.html` 本身無小智，未載入 xzm.js，僅同步版本。
- 版本 `v24-up1103-xz1103-xzm1103` 同步：`version.json`、`sw.js`、`index.html`／`繁體index.html`（APPVER、`upd321.js?v=`）、本 README。

## v24-up1103-xz1103（2026-11-03）自動更新（確認版）
- 原本 `sw.js` 為快取優先、改版全靠手動升快取號，且清快取時會刪光同網域所有 App 的快取。已改為正規自動更新：網路優先（HTML／JS／JSON）、只清自己前綴（`cc321-`、舊 `couples-321-v23`）的快取。
- 加入通用自動更新掛件 `upd321.js`：`version.json` 輪詢＋`reg.update()`，空閒時自動換新版，輸入中／朗讀中只顯示頂端更新條，結束後自動套用；防無限重整。「我們」頁新增「版本與更新」（檢查更新／強制更新）。`index.html` 與 `繁體index.html` 都已加入。
- 版本 `v24-up1103-xz1103` 四處一致：`version.json`、`sw.js`、`index.html`／`繁體index.html`（APPVER）、本 README。
- 註：本 repo 為夫妻成長營早期版本（現行為三語的 321couples），仍補上自動更新，避免已安裝的使用者卡在舊版。

