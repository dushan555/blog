# blog

首页是镜像站风格的 `public/` 目录列表：显示文件名、修改时间，点击文件直接访问，点击文件夹进入，`../` 返回上级。

把文件放到 `public/`，提交到 GitHub Pages 发布分支即可。Jekyll 在部署时自动收集资源，无需 Python 或手动维护清单。修改时间来自部署时的文件时间。

GitHub 仓库的 **Settings → Pages → Build and deployment** 应选择 **Deploy from a branch**，发布目录选择仓库根目录 **/ (root)**。每次提交后，等待 **pages build and deployment** 成功，再访问网站首页。

`index.html` 的前三行必须保留，它们是让 GitHub Pages 执行目录模板的构建配置，不会显示在部署后的网页上：

```yaml
---
layout: null
---
```

不要添加 `.nojekyll` 文件，否则会跳过模板处理。直接双击 HTML 或普通静态服务器不会执行 Jekyll 模板；本地预览可用 `jekyll serve`。
