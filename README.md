# 双面测试研究所

本仓库包含两个独立的、纯静态 HTML 娱乐测试网站，由 GitHub 管理源码，Cloudflare Pages 自动构建部署。

## 线上网址

| 网站 | 自定义域名 | Cloudflare Pages 项目 | 源码目录 |
| --- | --- | --- | --- |
| 李苛人格侧写 | https://personality.179652341.xyz | [li-ke-profile-site](https://li-ke-profile-site.pages.dev) | `serious/` |
| 你是什么类型的傻逼李苛？256 型鉴定局 | https://like.179652341.xyz | [li-ke-roast-site](https://li-ke-roast-site.pages.dev) | `roast/` |

这两个项目均关联 `tiantian185/gpt-web` 的 `main` 分支。Cloudflare Pages 每次检测到仓库更新会自动执行静态部署，不再使用单独的 Cloudflare Worker 进行网页托管。

## 目录结构

- `index.html`：两个测试的仓库导航首页
- `serious/index.html`：32 道情境题，每题 4 个行为选项；4 个维度各 3 档，共 81 种可命中的组合画像，含差异化结果解读、雷达图、分享和图片保存功能。
- `roast/index.html`：32 道日常翻车题，按工作、游戏、朋友社交、消费购物、生活习惯、网络冲浪、判断决策和日常人际 **8 类场景各 4 题** 均匀分配；四维各 8 题，每维 4 档，256 种可命中的“傻逼李苛”组合结果。结果文案同步聚焦日常行为。
- `README.md`：部署说明

## 修改和发布

1. 在 GitHub 修改 `serious/index.html` 或 `roast/index.html`，提交到 `main`。
2. Cloudflare Pages 的两个项目会从此仓库自动构建。
3. 源站 `*.pages.dev` 可供部署检查；两个自定义子域名 CNAME 分别指向其 Pages 域名。

人格问卷为娱乐用途，未经过临床、心理测量学验证。整蛊版中的辱骂和“鉴定”均为夸张的虚构笑话，请勿用于恶意骚扰或对现实人物作事实评价。
