# Waymark Preset Plugin

[Infiziert90/WaymarkPresetPlugin](https://github.com/Infiziert90/WaymarkPresetPlugin) 的台服移植版。
場地標記（A/B/C/D、1/2/3/4）預設集管理工具，可離線編輯、匯入匯出、依地圖／副本快速套用。

## 功能

- 建立、編輯、複製、刪除場地標記預設集，可視覺化在地圖上拖曳調整座標
- 依地圖分類的預設集清單，支援拖曳排序、搜尋篩選
- 一鍵把預設集寫進遊戲內建的場地標記保存欄位
- 與遊戲內建「場地標記」介面連動開關、可停靠在該介面旁
- 圓圈計算器：輸入圓心座標、半徑、點數與角度偏移，自動算出等距分布的標記點
- 支援匯入 / 匯出預設集字串，方便與他人分享
- 進入副本時可自動載入該地圖的預設集；離開時可自動把保存欄位的內容存回本插件
- 提供 IPC 供其他插件依地圖或副本查詢、套用預設集

## 使用

- `/pwaymark` 開啟主視窗（含子指令，詳見插件內說明）

## 台服版的修改

- 別的插件透過 IPC 放場地標記時，改成交回遊戲主執行緒執行，不再可能把遊戲弄崩
- 介面繁體中文化

## 安裝

在 Dalamud 設定的「自訂插件庫」加入
`https://raw.githubusercontent.com/ffxiv-tc-port/DalamudPluginsTC/main/repo.json` 並啟用，
再從插件列表安裝。

原作者：PunishedPineapple、[Infiziert90](https://github.com/Infiziert90)
