# 保時捷台灣庫存儀表板

公開網站，無需登入。展示台灣各保時捷中心掛在 [Porsche Finder](https://finder.porsche.com/tw/zh-TW?int_ref=globalnav&int_medium=link&int_id=inventory) 上的公開庫存、各車系占比，以及經銷商 × 車系矩陣，用來對照各店庫存、調整新車折扣。

- 網站：https://stanten1336.github.io/porsche-tw-inventory/
- 資料來源僅限 Porsche Finder 公開頁，不是全省每台實體車，也不是官方內部系統。
- 此儲存庫是**公開的**：任何人都可以看到網站程式碼與每日彙整的庫存資料。

## 更新方式

在資料機上執行：

```bash
python3 /workspace/porsche-finder/publish.sh
```

腳本會重新抓取當天庫存、寫入 `data.json`，若資料或頁面有變更就提交並推送到 `main`，GitHub Pages 會自動更新網站。
