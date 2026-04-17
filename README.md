# FitState AI Website

FitState AI 官方网站 - 使用 GitHub Pages 托管

## 网站结构

```
Website/
├── index.html          # 中文主页
├── index_en.html       # 英文主页
├── privacy.html        # 中文隐私政策
├── privacy_en.html     # 英文隐私政策
├── support.html        # 中文技术支持
├── support_en.html     # 英文技术支持
└── README.md           # 本文件
```

## 网址

- 主页: https://athenalion007.github.io/fitstate.ai
- 隐私政策: https://athenalion007.github.io/fitstate.ai/privacy.html
- 技术支持: https://athenalion007.github.io/fitstate.ai/support.html

## 部署到 GitHub Pages

### 步骤 1: 创建 GitHub 仓库

1. 登录 GitHub (https://github.com)
2. 点击右上角 "+" 号，选择 "New repository"
3. 仓库名称: `fitstate.ai`
4. 设置为 Public
5. 点击 "Create repository"

### 步骤 2: 上传文件

在终端中执行以下命令：

```bash
# 进入网站目录
cd /Users/macx/Documents/FitStateAI/Website

# 初始化 Git 仓库
git init

# 添加所有文件
git add .

# 提交更改
git commit -m "Initial commit: FitState AI website"

# 添加远程仓库（替换为你的 GitHub 用户名）
git remote add origin https://github.com/athenalion007/fitstate.ai.git

# 推送到 GitHub
git branch -M main
git push -u origin main
```

### 步骤 3: 启用 GitHub Pages

1. 进入 GitHub 仓库页面
2. 点击 "Settings" 标签
3. 左侧菜单选择 "Pages"
4. 在 "Source" 部分，选择 "Deploy from a branch"
5. 选择 "main" 分支，文件夹选择 "/ (root)"
6. 点击 "Save"

等待几分钟，网站将部署到：
`https://athenalion007.github.io/fitstate.ai`

### 步骤 4: 配置自定义域名（可选）

如果你有自定义域名 `fitstate.ai`：

1. 在 Website 目录下创建 `CNAME` 文件：
   ```bash
   echo "fitstate.ai" > CNAME
   git add CNAME
   git commit -m "Add custom domain"
   git push
   ```

2. 在你的域名 DNS 提供商处添加 CNAME 记录：
   - 主机记录: `@` 或 `www`
   - 记录类型: `CNAME`
   - 记录值: `athenalion007.github.io`

3. 在 GitHub Pages 设置中，在 "Custom domain" 部分输入 `fitstate.ai`，点击 "Save"

4. 勾选 "Enforce HTTPS"（推荐）

## 更新网站

修改文件后，执行：

```bash
cd /Users/macx/Documents/FitStateAI/Website
git add .
git commit -m "Update website content"
git push
```

更改将在几分钟内自动部署。

## 本地预览

在浏览器中打开文件即可预览：

```bash
open /Users/macx/Documents/FitStateAI/Website/index.html
```

或使用 Python 启动本地服务器：

```bash
cd /Users/macx/Documents/FitStateAI/Website
python3 -m http.server 8000
```

然后访问 http://localhost:8000

## 技术说明

- 纯静态 HTML/CSS，无需后端
- 响应式设计，适配移动端
- 支持中英文切换
- 使用 CSS 变量统一管理颜色主题
- 颜色方案与 FitState AI App 保持一致

## 颜色主题

| 颜色 | 色值 | 用途 |
|------|------|------|
| Primary | #1B4332 | 主色调（深绿色） |
| Secondary | #2C5F4C | 次要色 |
| Background | #F9FAFB | 背景色 |
| Card Background | #FFFFFF | 卡片背景 |
| Text Primary | #1D1D1F | 主要文字 |
| Text Secondary | #8E8E93 | 次要文字 |

## 联系信息

- 邮箱: support@fitstate.ai
- GitHub: https://github.com/athenalion007

---

© 2026 FitState AI. All rights reserved.
