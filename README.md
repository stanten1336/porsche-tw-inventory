# 保時捷台灣新車庫存儀表板

公開網站，無需登入。展示台灣各保時捷中心掛在 [Porsche Finder](https://finder.porsche.com/tw/zh-TW/search?condition=new) 上的**公開新車**庫存與車系占比，以及經銷商 × 車系矩陣，用來對照各店庫存、調整新車折扣。不含認證中古車與中古車。

- 網站：https://stanten1336.github.io/porsche-tw-inventory/
- 資料來源僅限 Porsche Finder 公開新車頁，不是全省每台實體車，也不是官方內部系統。
- 此儲存庫是**公開的**：任何人都可以看到網站程式碼與每日彙整的新車庫存資料。

## 更新方式

在資料機上執行：

```bash
/workspace/porsche-finder/publish.sh
```

腳本會重新抓取當天新車庫存、寫入 `data.json`、把當日彙整附加到 `history.json`，若資料或頁面有變更就提交並推送到 `main`，GitHub Pages 會自動更新網站。
