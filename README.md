# Table Tennis Arena｜桌球競技場

以 HTML、CSS 與 Canvas 製作的 2.5D 桌球遊戲，包含器材配置、旋轉與落點選擇，以及電腦對手。

## 開始遊玩

下載本專案後，直接用現代瀏覽器開啟 [`games/table-tennis-sim.html`](games/table-tennis-sim.html)。
桌球遊戲本體不需要安裝套件、執行建置或連接伺服器。

也可以先使用 Git 下載：

```sh
git clone https://github.com/JYC1224/tabletennisarena.git
cd tabletennisarena
```

## 操作

| 動作 | 操作方式 |
| --- | --- |
| 移動球拍 | 滑鼠、觸控、左右方向鍵或 A／D |
| 發球／擊球 | 點擊球檯、空白鍵或畫面上的擊球按鈕 |
| 選擇擊球方式 | 畫面按鈕或數字鍵 1–6 |
| 選擇落點 | 點擊左／中／右、長／短落點按鈕；Q／E 可左右切換 |

球在己方半檯落台後才能回擊。可使用搓球、擋球、快帶、弧圈、側旋與扣殺。
比賽採單局 11 分、領先 2 分獲勝，每 2 分換發，10:10 後每分換發。

## 器材配置

可分別選擇底板、正手膠皮與反手膠皮：

| 品牌 | 底板 | 膠皮 |
| --- | --- | --- |
| Butterfly 蝴蝶 | Viscaria | Tenergy 05 |
| Nittaku 妮塔庫 | Acoustic | Fastarc G-1 |
| JOOLA 尤拉 | Vyzaryz Freeze HRD | Dynaryz AGR |
| DONIC 多尼克 | Waldner Senso Carbon | BlueGrip C2 |
| STIGA 斯蒂加 | Clipper Wood | DNA Platinum H |

器材組合會影響遊戲中的球速、旋轉、容錯與弧線。型號與特性參考品牌官方資料，相關連結列在遊戲的「規則、器材來源與模擬說明」中。
0–100 數值是遊戲平衡估計值，並非跨品牌實測評分。球路使用簡化物理模型，未涵蓋完整空氣動力學、人體動作與裁判細則。

## 檔案

- `games/table-tennis-sim.html`：可獨立執行的桌球遊戲，包含畫面、操作與遊戲邏輯。
- `index.html`：原有的遊戲式學習介紹頁，也提供桌球遊戲入口。該頁其餘 Phaser 範例依賴相鄰的 `../phaser-examples/` 資料夾；這些範例不包含在本 repo 中。
