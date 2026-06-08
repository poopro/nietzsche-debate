# 與查拉圖斯特拉辯論

> **一場與尼采的文字辯論 RPG。**
> 靈感來自《極樂迪斯可》（Disco Elysium），由 AI 扮演查拉圖斯特拉，在哲學交鋒中勝過他。

這是一個**單一 HTML 檔**——下載 `index.html`，用瀏覽器打開即可遊玩。無需安裝、無需伺服器。
play demo here: https://brilliant-macaron-197e38.netlify.app/

---

## 快速開始

1. 用 Chrome / Edge / Firefox 打開 `index.html`
2. 到 [OpenRouter](https://openrouter.ai/) 註冊並建立 API Key（格式：`sk-or-v1-...`）
3. 在角色建立畫面貼上 Key，點擊「測試連接」
4. 創建角色，開始辯論

**注意：** 查拉圖斯特拉的台詞、選項回饋與裁判報告均由 OpenRouter AI 生成，沒有 API Key 無法正常遊玩。

---

## 遊戲特色

- **⌬ 四項技能系統** ―― 邏輯（紅）/ 直覺（藍）/ 情感（綠）/ 辯才（黃），每次辯論有不同路線
- **⌬ 思維卡牌系統** ―― 類似「技能牌組」，構成你的內在哲學立場
- **⌬ AI 對手** ―― 查拉圖斯特拉由 OpenRouter 驅動，每次辯論都不一樣
- **⌬ 裁判報告** ―― 每局結束後 AI 生成正式的勝負裁決
- **⌬ 本地存檔** —— 所有進度存在 `localStorage`，不上傳任何伺服器

---

## 文件結構

```
nietzsche-debate/
├── index.html      # 遊戲本體（唯一必要檔案）
├── README.md       # 本文件
└── 遊玩指南.md     # 完整遊戲說明（含技能、卡牌、UI、操作手冊）
```

---

## 系統需求

- 現代瀏覽器（Chrome / Edge / Firefox）
- OpenRouter API Key
- 建議螢幕寬度 ≥ 900px（窄螢幕側欄會自動隱藏，核心對話區仍可用）

---

## 技術細節

- 純前端：零依賴，單一 HTML 檔案
- 型號：`louise`（OpenRouter 端點存檔）用於遊戲內關鍵字偵測
- 所有 API 請求經由 `maxLength` 與 `temperature` 控制

---

## 授權

本專案採用 GNU Affero General Public License v3.0 —— 詳情見 [LICENSE](https://www.gnu.org/licenses/agpl-3.0.html) 或下方摘要：

> 本程式的版權持有人允許任何人在相同條款下使用、修改與分發本軟體，**包括網路服務**。如果你修改了本軟體並提供網路服務，你必須公開修改後的源程式碼。這保障使用者查看、修改的自由，也保障這項自由能延續到衍生作品中。

---

*查拉圖斯特拉下了山。這次，你不打算只是聽他說話。*
