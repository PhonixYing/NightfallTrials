# Nightfall Trials 官网

这是一个无需构建步骤的静态官网，可直接部署到 GitHub Pages。

## 本地预览

在本目录执行：

```bash
python3 -m http.server 8080
```

然后打开 `http://localhost:8080`。

## 部署到 GitHub Pages

1. 在 GitHub 创建仓库，例如 `nightfall-trials`。
2. 将此目录中的全部文件推送到仓库根目录（或推送到单独的 `docs/` 目录）。
3. 打开仓库 **Settings → Pages**。
4. 在 **Build and deployment** 中选择 `Deploy from a branch`。
5. 选择 `main` 分支，并选择 `/ (root)`（若文件放在 `docs` 则选择 `/docs`），点击 **Save**。
6. 等待部署完成后，GitHub 会显示站点 URL。

## 上线前替换项

- 在 `index.html` 中把 “Mac App Store 即将上线” 链接换为真实 App Store URL。
- 在 `privacy.html` 中补充实际的开发者联系邮箱或 GitHub 仓库 URL。
- 需要自定义域名时，在仓库 Settings → Pages 填入域名，并在 DNS 添加 GitHub Pages 所需记录。

站点没有框架、包依赖或服务端；适合 GitHub Pages 的纯静态托管。
