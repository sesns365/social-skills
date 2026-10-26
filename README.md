# 社交小特工教材包

國小社會技巧動畫系列「社交小特工」的教材包網站，由特工365 製作。每集提供互動網頁（內嵌動畫與 8 題測驗）、A／B／C 學習單（PDF 與 docx）、教學指引，課堂免費使用。

網站：https://sesns365.github.io/social-skills/

## 資料夾結構

```
index.html            首頁、單集頁、教師使用說明、課綱對照（同一個檔案，用 #ep1 等切換）
ep1/
  interactive.html    第 1 集互動網頁
  worksheet-A.pdf     學習單 A 版（圖片勾選）
  worksheet-A.docx
  worksheet-B.pdf     學習單 B 版（句型填空）
  worksheet-B.docx
  worksheet-C.pdf     學習單 C 版（情境書寫）
  worksheet-C.docx
  guide.pdf           教學指引（完成後放上）
  poster.pdf          選配：口訣海報
  cards.pdf           選配：策略卡
  record.pdf          選配：評量紀錄表
```

動畫 MP4 不放在這裡，改連 YouTube。

## 新增一集的步驟

1. 建立 `epN/` 資料夾，放入 `interactive.html`、`worksheet-A/B/C.pdf`、`worksheet-A/B/C.docx`，有教學指引再放 `guide.pdf`，有選配材料再放 `poster.pdf`、`cards.pdf`、`record.pdf`。
2. 在 `index.html` 的 `EPS` 清單把第 N 集狀態改為 `ok`。集數依課綱學習內容代碼的字母自動分組（A 處己、B 處人、C 處環境），不用另外設定。
3. 複製第 1 集的單集頁區塊（`id="v-ep1"`）改成第 N 集內容，並在 `VIEWS` 加上 `epN`。
4. 影片上架後，把 YouTube 按鈕換成影片連結與章節時間。
5. 推上 `main` 分支，GitHub Pages 約 1 分鐘後更新。
