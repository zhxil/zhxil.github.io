# 用 Codex 一键部署 zhxil.github.io

目标仓库：`https://github.com/zhxil/zhxil.github.io`
上线地址：`https://zhxil.github.io`

本包的 `index.html` 必须直接位于仓库根目录（不是再套一层 `site`）。

## 使用方法（Windows）

1. 解压本 ZIP 到本地文件夹，例如 `D:\WorkSpace\zhxil.github.io`。
2. 在此文件夹打开 Codex（CLI / IDE 插件均可）。
3. 将下方【交给 Codex 的指令】完整发送给 Codex。
4. GitHub Pages 首次开启可能需要到仓库 Settings → Pages 中手动选一次「Deploy from a branch / main / /(root)」。之后提交到 main 会自动部署。

## 交给 Codex 的指令

请把当前文件夹中已经准备好的静态个人网站部署到我的 GitHub 仓库：
https://github.com/zhxil/zhxil.github.io

我的 GitHub 用户名是 zhxil，仓库已创建，目标网址是 https://zhxil.github.io。

请按以下步骤实际执行，遇到需要我授权或登录时再让我操作：
1. 检查当前目录包含 index.html、assets/、projects/ 和 .nojekyll，不要自行重做页面。
2. 本地检查 index.html 与四个 projects/*.html 的相对链接和资源引用，检查是否有明显错误。
3. 检查 git、gh 是否可用；若有 GitHub 身份验证，直接复用，绝不索要或输出个人访问令牌。
4. 检查目标仓库当前内容与本地 Git 状态。仓库为空则初始化 main 并设 origin；如果已经存在代码，先拉取和审查差异，禁止 force push、禁止覆盖不相关数据。
5. 将网站文件（不是压缩包）提交并推送到 `zhxil/zhxil.github.io` 的 main 分支。忽略本地缓存、机密和临时文件。
6. 检查 GitHub Pages 是否启用。优先使用 GitHub CLI/API 尝试将 source 配置为 main 分支的 /(root)。如果 API 没有权限，明确告诉我需要手动进入 Settings → Pages 设置，不要假装已成功。
7. 检查 https://zhxil.github.io 能否打开，并检查四个项目详情页面；部署有延迟可合理等待重试。如果尚未部署成功，给出具体错误和下一步。

请尽量直接执行，不要仅生成方案。最后反馈仓库提交 SHA、GitHub Pages 状态、最终网站网址，以及是否需要我手动操作。

## 如果需要手动开启 GitHub Pages

进入：
https://github.com/zhxil/zhxil.github.io/settings/pages

在 **Build and deployment** 中选择：
- Source: Deploy from a branch
- Branch: main
- Folder: /(root)

保存后等待 GitHub Pages 发布，再访问 https://zhxil.github.io。

## 注意事项

- 网站完全静态，无需 npm、Python 环境或服务器才能上线。
- `assets/style.css` 控制全站样式，`assets/site.js` 控制交互。
- 四个项目分别为 CodexWatch、iPhoneStock、LumaConvert 和 ContentFactory。
- 部分项目截图使用 GitHub 仓库 raw 图片链接，需要访客可访问 GitHub 的图片资源。
- 保持 iPhoneStock 详情页中的第三方协议与许可归属说明。
- 不要向站点发布 API Key、密码、SSH 私钥、含个人敏感信息的配置文件。
