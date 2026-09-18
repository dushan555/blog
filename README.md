# blog

首页是镜像站风格的 `public/` 目录列表：显示文件名、修改时间，点击文件直接访问，点击文件夹进入，`../` 返回上级。

把文件放到 `public/`，提交到 GitHub Pages 发布分支即可。Jekyll 在部署时自动收集资源，无需 Python 或手动维护清单。修改时间来自部署时的文件时间。

`index.html` 开头的 YAML front matter（两行 `---` 及其中的配置）必须保留，否则 GitHub Pages 不会处理目录模板。直接双击 HTML 或普通静态服务器不会执行 Jekyll 模板；本地预览可用 `jekyll serve`。
