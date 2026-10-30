# shi-yi-shi

个人博客 · 记录 CTF / 密码学 / 嵌入式开发

## 技术栈

- 静态站点生成：[Hugo](https://gohugo.io/) v0.169.0 extended
- 主题：[PaperMod](https://github.com/adityatelange/hugo-PaperMod)
- 托管：Cloudflare Pages（免费二级域名 `shi-yi-shi.pages.dev`）

## 本地预览

```bash
cd D:/ADongjiayi/work/blog-shi-yi-shi
D:/ADongjiayi/study/hugo/hugo.exe server -D
```

浏览器打开 <http://localhost:1313/>。

## 新建一篇文章

```bash
D:/ADongjiayi/study/hugo/hugo.exe new content posts/我的第一篇.md
```

然后编辑 `content/posts/我的第一篇.md`，把 `draft = true` 改成 `draft = false`。

## 构建发布

```bash
D:/ADongjiayi/study/hugo/hugo.exe --minify
```

产物在 `public/` 目录，部署到 Cloudflare Pages 会自动构建（也可以直接推 `public/`）。

## 目录说明

```
content/          文章与页面
  posts/          博文
  about.md        关于页
  archives.md     归档
  search.md       搜索
themes/PaperMod/  主题（官方版，勿改）
hugo.toml         站点配置
```

## 改站点地址

部署到别的域名时，改 `hugo.toml` 第一行的 `baseURL` 即可。
