# 双面测试研究所

本仓库包含两个独立的、纯静态 HTML 娱乐测试网站，由 GitHub 管理源码，Cloudflare Pages 自动构建部署。

## 线上网址

| 网站 | 自定义域名 | Cloudflare Pages 项目 | 源码目录 |
| --- | --- | --- | --- |
| 李苛人格侧写 | https://personality.179652341.xyz | [li-ke-profile-site](https://li-ke-profile-site.pages.dev) | `serious/` |
| 你是哪种傻逼？256 型鉴定局 | https://like.179652341.xyz | [li-ke-roast-site](https://li-ke-roast-site.pages.dev) | `roast/` |

这两个项目均关联 `tiantian185/gpt-web` 的 `main` 分支。Cloudflare Pages 每次检测到仓库更新会自动执行静态部署，不再使用单独的 Cloudflare Worker 进行网页托管。

## 目录结构

- `index.html`：两个测试的仓库导航首页
- `serious/index.html`：24 道人格行为问卷、四维分数、结果卡片及分享功能
- `roast/index.html`：32 道荒诞整蛊题、四种行为强度、256 种独立组合的趣味结果（4 维度 × 各 4 档）。所有组合均可通过特定作答方式命中。
- `README.md`：部署说明

## 修改和发布

1. 在 GitHub 修改 `serious/index.html` 或 `roast/index.html`，提交到 `main`。
2. Cloudflare Pages 的两个项目会从此仓库自动构建。
3. 源站 `*.pages.dev` 可供部署检查；两个自定义子域名 CNAME 分别指向其 Pages 域名。

人格问卷为娱乐用途，未经过临床、心理测量学验证。整蛊版中的辱骂和“鉴定”均为夸张的虚构笑话，请勿用于恶意骚扰或对现实人物作事实评价。
