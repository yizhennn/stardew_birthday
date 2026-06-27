# 🌾 Stardew Valley 生日日報

鵜鶘鎮（Pelican Town）村民生日 / 節日查詢小工具，純前端打包，輸入季節與日期即可看到當天、本週、本季的生日與節慶活動，並附上每位村民的禮物喜好與好感度資訊。

GitHub：https://github.com/yizhennn/stardew_birthday

## 功能

- 📅 **今天** — 顯示所選日期的生日村民與節日活動
- 🗓 **本週** — 查看接下來一週的生日與活動
- 📆 **本季** — 整季生日／節慶總覽
- 👥 **村民** — 所有村民的好感度指南，含禮物喜好（最愛 / 喜歡 / 普通 / 不喜歡 / 討厭）
- 🔍 **搜尋** — 依中文或英文名稱搜尋村民或節日（例如：阿比蓋爾、Abigail、蛋蛋節）
- 🎁 送禮效果計算（含生日當天加成）與好感度里程碑提示

## 使用方式

這是純靜態網頁專案，需透過本地伺服器開啟（`stardew_data.json` 以 `fetch` 載入，直接用 `file://` 開啟會被瀏覽器擋掉）：

```bash
# 任選一種方式啟動本地伺服器，於專案根目錄執行
python -m http.server 8000
# 或
npx serve .
```

然後在瀏覽器開啟 `http://localhost:8000`。

## 專案結構

```
stardew_birthday/
├── index.html              # 主頁面（HTML + CSS + JS 全部打包在一起）
└── stardew/
    ├── stardew_data.json    # 生日、節慶資料
    ├── characters/          # 村民頭像
    ├── events/               # 節慶活動圖片
    └── items/                # 禮物道具圖片
```

## 技術

純 HTML / CSS / JavaScript，無任何框架或建置工具，資料以 JSON 靜態檔提供。

## 免責聲明

本專案為**非營利、非官方**的玩家自製輔助工具，僅供個人查詢遊戲內生日／節慶／禮物資訊之用，與 ConcernedApe LLC（《星露谷物語》開發商）**無任何關聯、未經其授權或認可**。

《星露谷物語》（Stardew Valley）及其角色、物品、美術等相關內容之版權均屬 ConcernedApe LLC 所有。專案中使用之村民頭像、物品與節慶圖示，取自 [Stardew Valley Wiki](https://stardewvalleywiki.com/) 作為遊戲內容識別之參考用途，所有權利仍歸原版權方所有。本專案不會、亦不打算用於任何商業用途。

如版權方或 Stardew Valley Wiki 認為任何內容的使用方式不妥，請告知並將立即配合移除。
