# 台股兵法智謀全媒體觀測系統（GitHub Pages 版）

這是可直接部署到 **GitHub Pages** 的版本，已完成以下調整：

- `vite.config.ts` 已改成 `base: './'`
- 已加入 GitHub Actions 自動部署設定
- 推到 GitHub 後可直接用 **GitHub Pages** 發佈

## 本機測試
```bash
npm install
npm run dev
```

## 本機建置
```bash
npm run build
```

## 發佈到 GitHub Pages
1. 建立新的 GitHub Repository
2. 把本專案全部檔案上傳到 Repository 根目錄
3. 到 GitHub 的 **Settings > Pages**
4. 在 **Build and deployment** 選擇 **GitHub Actions**
5. 確認預設分支為 `main`
6. 之後每次 push 到 `main`，就會自動部署

## 重要檔案
- `src/App.tsx`：主畫面
- `vite.config.ts`：已設定 GitHub Pages 相對路徑
- `.github/workflows/deploy-pages.yml`：自動部署流程
