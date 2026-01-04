# Data Analyst Portfolio Template

这是一个专为数据分析师/商业分析师设计的现代个人作品集网页模版。它采用 HTML5、CSS3 和少量 JavaScript 构建，设计风格简洁、专业且具有深色模式的科技感。

## ✨ 特性

- **现代深色主题**：符合数据可视化和科技领域的审美。
- **响应式设计**：完美适配手机、平板和桌面端。
- **动效交互**：平滑的滚动效果、悬浮预览和入场动画。
- **易于定制**：代码结构清晰，注释详细，方便修改内容。

## 📁 项目结构

```
YY_Portfolio/
├── index.html       # 主网页文件（你需要修改这里的内容）
├── css/
│   └── style.css    # 样式表（可以修改颜色和布局）
├── js/
│   └── main.js      # 交互脚本（通常不需要修改）
├── assets/          # 存放简历文件 (resume.pdf)
└── images/          # 存放项目图片和个人照片
```

## 🛠️ 修改指南

### 1. 修改个人信息
打开 `index.html`，搜索以下关键词进行替换：
- `[Your Name]` -> 替换为你的名字（多处）。
- `Data Analyst & Business Intelligence Pro` -> 替换为你的职位标题。
- `https://linkedin.com/in/yourprofile` -> 替换为你的 LinkedIn 链接。
- `https://github.com/yourusername` -> 替换为你的 GitHub 链接。
- `your.email@example.com` -> 替换为你的邮箱。

### 2. 添加简历
1. 将你的简历重命名为 `resume.pdf`。
2. 将其放入 `assets/` 文件夹中。
3. 如果文件名不同，请在 `index.html` 中找到 `Download Resume` 按钮，修改 `href="assets/resume.pdf"` 为你的文件名。

### 3. 修改“关于我” (About Me)
在 `index.html` 中找到 `<section id="about" ...>`：
- 修改 `<p>` 标签内的自我介绍。
- 在 `Tech Stack` 部分，你可以添加或删除技能。例如：
  ```html
  <div class="skill-item"><i class="fas fa-database"></i> SQL</div>
  ```
  *提示：可以在 [FontAwesome](https://fontawesome.com/search?o=r&m=free) 查找更多图标代码。*

### 4. 添加你的项目 (Portfolio)
在 `<section id="portfolio" ...>` 中，每个项目都在 `<div class="project-card">` 内。
复制一个 `project-card` 块来添加新项目，或者直接修改现有的：
- **图片**：修改 `src` 属性，指向你的图片（建议将图片放在 `images/` 文件夹，例如 `src="images/project1.png"`）。
- **标题与描述**：修改 `<h3>` 和 `<p>` 内容。
- **链接**：修改 `View Dashboard` 或 `View Code` 的 `href` 链接。

### 5. 修改头像 (可选)
如果你想在 About 部分显示照片，请取消注释 `index.html` 第 97-99 行的代码，并将你的照片放入 `images/` 文件夹。

---

## 🚀 部署到 GitHub Pages

GitHub Pages 是一个免费托管静态网页的服务，非常适合托管此类作品集。

### 第一步：准备 GitHub 仓库
1. 登录 [GitHub](https://github.com/)。
2. 点击右上角的 **+** 号，选择 **New repository**。
3. Repository name 填写 `portfolio` (或者 `yourusername.github.io` 如果这是你的主页)。
4. 确保选择 **Public**。
5. 点击 **Create repository**。

### 第二步：上传代码
如果你安装了 Git，请在项目文件夹根目录打开终端（Terminal/Git Bash）并运行：

```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/你的用户名/你的仓库名.git
git push -u origin main
```

**如果你不熟悉命令行**，也可以直接在 GitHub 网页上点击 "uploading an existing file"，将所有文件（保持文件夹结构）拖拽上传。

### 第三步：开启 GitHub Pages
1. 在你的 GitHub 仓库页面，点击 **Settings** (设置)。
2. 在左侧菜单找到 **Pages**。
3. 在 **Build and deployment** 下的 **Source** 选择 `Deploy from a branch`。
4. 在 **Branch** 下拉菜单选择 `main`，文件夹选择 `/ (root)`，然后点击 **Save**。
5. 等待几分钟，刷新页面，你会看到顶部出现你的网站链接（通常是 `https://你的用户名.github.io/仓库名/`）。

🎉 恭喜！你的个人作品集网站已经上线了！
