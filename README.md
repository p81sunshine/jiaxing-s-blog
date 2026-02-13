# Hacker Style Personal Blog

一个可部署到 GitHub Pages 的个人博客模板（Jekyll + `jekyll-theme-hacker`）。

## 页面

- 首页：`/`
- 文章列表：`/posts/`
- 分类：`/categories/`
- 标签：`/tags/`
- 关于：`/about/`

座右铭已内置在首页：**我思，故我在**。

## 本地运行

```bash
bundle install
bundle exec jekyll serve
```

默认本地地址：`http://127.0.0.1:4000`

## 部署到 GitHub Pages

1. 新建 GitHub 仓库并推送本项目代码到 `main` 分支。
2. 打开仓库 `Settings -> Pages`。
3. 在 `Build and deployment` 中选择 `GitHub Actions`。
4. 推送后会自动执行 `.github/workflows/pages.yml` 并发布。

## 个性化

- 修改站点信息：`_config.yml`
- 修改导航/页面内容：`index.md`、`posts.md`、`categories.md`、`tags.md`、`about.md`
- 修改视觉风格：`assets/css/style.scss`
- 发布你的文章：`_posts/*.md`
