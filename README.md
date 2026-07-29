# 道源符體 · 法本

符籙風格中文字體的展示頁。輸入文字，挑法式與紙色，即時排成符紙，可存成 PNG。

字體又稱雨君鬼臣體，思源黑體的衍生字體，把道教符籙的筆畫元素接在漢字字形上。字體由 [Losketch](https://github.com/Losketch/daoist-sigi-source) 製作，本 repo 只是它的展示頁。

## 功能

- **法式**：立符（直排）／橫符（橫排）
- **朱印**：硃砂、墨、金、素
- **紙**：黃籙、宣紙、墨底
- **法印**：敕令、敕雷令、急急如律令、無
- **字級／行距／字距／行長**滑桿即時調整，行長拉到底就不換行
- **缺字偵測**：同一個字用「符體＋備援」與「純備援」各畫進 canvas 比對像素，字集沒收的字會標出來並退回系統字體
- **下載 PNG**：符紙連暗紋、法印一起輸出
- **字表**：列出目前字集實際涵蓋的字

## 本機預覽

```bash
python3 -m http.server 8000
# → http://127.0.0.1:8000/
```

完整字集從 jsDelivr 取，網址釘在 `sigi.woff2` 所在的 commit（`@main` 的邊緣快取有 12 小時，釘 commit 才拿得到 immutable 的一年快取）。所以預覽要連網，離線時頁面會退回同目錄的 `sigi-lite.woff2`（513 字精簡字集）。

## 授權

字體 **道源符體（Daoist Sigi Source）** 版權為 © 2024 Lochen Sans / [Losketch](https://github.com/Losketch/daoist-sigi-source) 所有，採 SIL Open Font License 1.1 授權，全文見 `OFL.txt`。本 repo 收錄的版本為 release V1.000。

保留字體名稱（Reserved Font Names）為 “Daoist Sigi Source”、“道源符体”、“雨君鬼臣体”。本 repo 未改動字體輪廓，`sigi.woff2` 與 `sigi-lite.woff2` 都直接來自原字體，因此沿用原名。若你要改造字體再散布，依 OFL 條款必須改用其他名稱，並同樣以 OFL 1.1 釋出。
