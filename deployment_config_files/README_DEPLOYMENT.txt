Shadow Puppet Interactive Game - 專案發布與部署配置說明
=====================================================

本壓縮包包含可直接匯入/加入您專案庫（bijue113045-droid/Shadow-Puppet-Interactive-Game-2）的完整部署設定檔：

1. .github/workflows/deploy.yml
   - GitHub Pages 自動化部署工作流程 (CI/CD)。
   - 放置於專案根目錄 `.github/workflows/` 資料夾內。
   - 推送至 main 分支時會自動編譯並發布到 GitHub Pages。

2. vercel.json
   - Vercel 部署設定檔。
   - 放置於專案根目錄，導入 Vercel 時將自動辨識 Vite 專案設定與單頁應用 (SPA) 路由。

3. netlify.toml
   - Netlify 部署設定檔。
   - 放置於專案根目錄，自動設定構建指令 (npm run build) 與重定向規則。

4. Dockerfile
   - 適用於 Docker / Cloud Run / VPS 容器化部署。
   - 使用多階段構建 (Multi-stage build)，編譯後交由 Nginx 提供靜態網頁服務。

使用方式：
解壓縮後將對應檔名之檔案直接複製並 Commit 到您的 GitHub 專案庫中即可！
