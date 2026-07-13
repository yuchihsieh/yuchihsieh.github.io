# yuchihsieh — academic website

一頁式學術個人網站（純 HTML，沒有 build step）。

## 還缺的素材（填進 `index.html` 裡的 TODO）

1. `photo.jpg` — LinkedIn 用的那張照片，放在 repo 根目錄
2. 已發表 paper 的：標題、合著者、期刊、年份、連結
3. 2–3 篇 working paper 的標題
4. LinkedIn / Google Scholar 連結（沒有的刪掉即可）
5. `cv.pdf`（可選，沒有就把 CV 連結刪掉）

## 上線步驟（GitHub Pages）

1. 把這個 branch merge 進 `main`
2. GitHub repo → **Settings → Pages** → Source 選 `main` branch、`/ (root)`
3. 幾分鐘後網站就在 `https://yuchihsieh.github.io/website/`
   - 想要乾淨的 `https://yuchihsieh.github.io/`，把 repo 改名成 `yuchihsieh.github.io` 即可

## 自訂網域 `yuchihsieh.tw`（可以之後再弄，不擋上線）

1. 註冊網域（Gandi、PChome 買網址等 TWNIC 註冊商都可以，.tw 約 NT$800/年）
2. DNS 設定：
   - `A` 記錄指向 GitHub Pages 的四個 IP：`185.199.108.153`、`185.199.109.153`、`185.199.110.153`、`185.199.111.153`
   - `www` 的 `CNAME` 指向 `yuchihsieh.github.io`
3. repo → Settings → Pages → Custom domain 填 `yuchihsieh.tw`，勾選 Enforce HTTPS
4. DNS 生效通常幾分鐘到幾小時；HTTPS 憑證由 GitHub 自動簽發
