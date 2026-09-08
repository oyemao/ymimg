# img-bed · 个人免费图床

GitHub + jsDelivr 免费图床空间，图片统一存放在 `images/` 目录。

## jsDelivr CDN 链接格式

```
https://cdn.jsdelivr.net/gh/oyemao/img-bed@main/images/<文件名>
```

例如上传 `images/2026/hello.png` 后，访问链接为：

```
https://cdn.jsdelivr.net/gh/oyemao/img-bed@main/images/2026/hello.png
```

## 特性

- 免费：GitHub 仓库存储 + jsDelivr 全球 CDN 加速，零成本
- 稳定：jsDelivr 自带多节点缓存与故障转移
- 简单：用配套 GUI 上传工具（`imgbed_uploader.py`）一键上传并复制链接

## 使用说明

1. 本仓库为**公共仓库**（jsDelivr 仅加速公共仓库），请勿存放隐私/敏感图片。
2. 单文件建议不超过 20 MB（GitHub API 上限）。
3. 上传方式：
   - 使用本仓库配套的 GUI 工具（推荐）：选择图片 → 自动上传 → 复制 jsDelivr 链接
   - 或直接 `git push` 到 `main` 分支

## 注意

- 新上传的文件 jsDelivr 首次访问需几秒拉取，之后走 CDN 缓存。
- 删除文件后 CDN 缓存最长 7 天失效，请谨慎删除已引用图片。
