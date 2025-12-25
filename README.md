# liam798.github.io

该仓库使用 [VitePress](https://vitepress.dev) 构建个人主页，开发与部署流程如下：

- 本地调试：运行 `pnpm dev`（或 `pnpm run dev`）即可实时预览 `docs/` 下的文档内容。
- 构建产物：执行 `pnpm build` 生成静态文件，输出目录位于 `docs/.vitepress/dist`。
- 自动部署：向 `main` 分支推送代码后，GitHub Actions 会执行 `.github/workflows/deploy.yml`，将构建产物发布到 `gh-pages` 分支供 GitHub Pages 使用。

首次配置时，请在 GitHub 仓库的 Pages 设置中选择 `gh-pages` 分支的 `/(root)` 作为发布源，之后 Action 将自动更新页面。
