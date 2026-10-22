# 認識多元的世界

三段 3D 第一人稱體驗，讓國中生走進三位同學的一天，感受每個人接收世界的方式都不一樣，再想想環境和身邊的人可以怎麼調整。

線上體驗：https://chuoneone.github.io/diverse-world/

## 內容

| 檔案 | 內容 |
|---|---|
| `index.html` | 遊戲主選單、選擇關卡、暖身、給帶領的老師 |
| `loud-day.html` | 世界太大聲的一天：聲音、光線、字面理解、計畫改變 |
| `focus-day.html` | 分心的第一天：注意力被拉走、記不住交代、衝動 |
| `reading-day.html` | 小安的開學日：字會跳動、聽不完整、數字翻面、抄寫 |

## 想改編？

歡迎自由改編，直接 fork 或 clone 即可，不需要安裝任何東西。

```bash
git clone https://github.com/chuoneone/diverse-world.git
cd diverse-world
python -m http.server 8000
```

打開 http://localhost:8000 就能看到。也可以直接用瀏覽器開啟 `index.html`。

### 發布成自己的網站

1. 在 GitHub 按 **Fork**。
2. 到你 fork 的 repo：Settings → Pages，Source 選 `main` 分支、`/ (root)`。
3. 一分鐘左右，網址會是 `https://你的帳號.github.io/diverse-world/`。

### 修改前先知道

- 每個檔案都是單一 HTML，程式、畫面和特效都寫在裡面，沒有建置步驟。四個檔案之間互相獨立，改一個不會影響其他。
- 需要連網：three.js 和中文字體是從 CDN 載入的。
  - `loud-day.html` 使用 three.js 0.149（jsDelivr）。
  - 其他三個檔案使用 three.js r128（cdnjs）。
  - 兩個版本的寫法不完全相同，程式碼不能直接在檔案之間複製貼上。
- 關卡的「已完成」記錄只存在使用者自己的瀏覽器（`localStorage`），不會上傳任何資料。

### 改編時請保留的原則

這不是授權條件，是創作時的初衷，請改編的人盡量維持：

- **不貼標籤**：不在遊戲中指名特定的障別或診斷，只描述感受和需要。
- **看見環境**：讓玩的人看到「環境調整」帶來的差別，而不是把困難歸給個人。
- **問本人**：提醒玩的人，每個人都不一樣，想了解就問本人。

## 授權與出處標示

本作品以 [CC BY 4.0（姓名標示 4.0 國際）](https://creativecommons.org/licenses/by/4.0/deed.zh_TW) 授權，完整條款見 [`LICENSE`](LICENSE)。你可以分享、改編、用於教學或商用，只要註明出處並說明是否有修改。

建議的出處寫法：

> 改編自「認識多元的世界」（chuoneone，https://github.com/chuoneone/diverse-world），CC BY 4.0。

第三方項目維持各自的授權：three.js（MIT）、Noto Sans TC、Iansui、LXGW WenKai TC（SIL Open Font License）。

## 注意

遊戲中的人物和情境都是虛構的，只模擬部分經驗，不能代表任何一個人，也不能用來判斷別人。
