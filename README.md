# GitHub Desktop 中文版指南

本仓库是 GitHub Desktop（GitHub 官方桌面客户端）的中文使用指南，将所有界面菜单、按钮、操作流程翻译成中文，帮助你快速上手。

> GitHub Desktop 本身没有官方中文语言包，本指南通过界面翻译对照和操作教程，让你像用中文版一样使用它。

## 目录

- [界面中文对照](#界面中文对照)
- [快速入门](#快速入门)
- [基本操作](#基本操作)
- [分支管理](#分支管理)
- [常见问题](#常见问题)

---

## 界面中文对照

### 菜单栏

| 英文 | 中文 | 说明 |
|------|------|------|
| **File** | 文件 | 文件相关操作 |
| → Options | → 选项 | 设置窗口 |
| → Add Local Repository | → 添加本地仓库 | 将已有文件夹加入 GitHub Desktop |
| → Clone Repository | → 克隆仓库 | 从 GitHub 远程克隆 |
| → New Repository | → 新建仓库 | 在本地创建新仓库 |
| **Edit** | 编辑 | 编辑操作 |
| → Undo | → 撤销 | 撤销上一步操作 |
| → Redo | → 重做 | 重做撤销的操作 |
| **View** | 视图 | 界面视图切换 |
| → Toggle Full Screen | → 切换全屏 | 全屏显示 |
| → Zoom In | → 放大 | 界面放大 |
| → Zoom Out | → 缩小 | 界面缩小 |
| → Actual Size | → 恢复默认大小 | 重置缩放 |
| → Show Changes | → 显示更改 | 查看文件改动 |
| → Show History | → 显示历史 | 查看提交记录 |
| **Repository** | 仓库 | 仓库相关操作 |
| → Repository Settings | → 仓库设置 | 仓库配置 |
| → Add Remotes | → 添加远程仓库 | 关联远程地址 |
| → Open in Command Prompt | → 在命令提示符中打开 | 打开终端 |
| → Open in Visual Studio Code | → 在 VS Code 中打开 | 用编辑器打开项目 |
| → Push | → 推送 | 提交推送到远程 |
| → Pull | → 拉取 | 从远程拉取最新代码 |
| **Branch** | 分支 | 分支管理 |
| → New Branch | → 新建分支 | 创建新分支 |
| → Merge Branch into Current | → 合并分支到当前分支 | 合并代码 |
| → Rename Branch | → 重命名分支 | 改分支名 |
| → Delete Branch | → 删除分支 | 删除分支 |
| → Compare Branch to... | → 比较分支... | 查看分支差异 |
| **Help** | 帮助 | 帮助信息 |
| → Documentation | → 文档 | 官方文档 |
| → Support | → 支持 | 获取帮助 |
| → About GitHub Desktop | → 关于 GitHub Desktop | 版本信息 |

### 主界面按钮对照（欢迎页）

| 英文 | 中文 | 说明 |
|------|------|------|
| **Let's get started!** | 开始使用！ | 欢迎页标题 |
| Add a repository to GitHub Desktop to start collaborating | 将仓库添加到 GitHub Desktop 以开始协作 | 欢迎页说明文字 |
| **Filter your repositories** | 筛选你的仓库 | 仓库搜索框 |
| **Create a tutorial repository...** | 创建一个教程仓库... | 自动生成练习用仓库 |
| **Clone a repository from the Internet...** | 从网络克隆仓库... | 从 GitHub 远程拉取 |
| **Create a New Repository on your local drive...** | 在本地磁盘创建新仓库... | 新建本地仓库 |
| **Add an Existing Repository from your local drive...** | 从本地磁盘添加已有仓库... | 导入已有文件夹 |
| **ProTip!** | 小技巧！ | 提示信息 |
| You can drag & drop an existing repository folder here to add it to Desktop | 你可以直接拖放已有仓库文件夹到这里来添加 | 拖放提示 |
| Refresh this list | 刷新此列表 | 刷新仓库列表链接 |

---

## 快速入门

### 第一步：添加仓库

打开 GitHub Desktop 后，你会看到欢迎页。根据你的情况选择：

- **第一次用**：点击 `Create a tutorial repository...`（创建一个教程仓库），GitHub Desktop 会自动生成一个练习仓库
- **已有远程仓库**：点击 `Clone a repository from the Internet...`（从网络克隆仓库）
- **已有本地项目**：点击 `Add an Existing Repository from your local drive...`（从本地磁盘添加已有仓库）

### 第二步：认识主界面

添加仓库后，主界面分为以下区域：

| 区域 | 中文名称 | 位置 | 功能 |
|------|------|------|------|
| 左侧 | 仓库列表 | 左上角 | 切换不同仓库 |
| 左侧 | 分支选择器 | 仓库名下方 | 切换当前分支 |
| 中间上方 | 更改面板 | 左侧主区域 | 查看修改的文件 |
| 中间下方 | 提交信息 | 更改面板下方 | 输入提交说明 |
| 右侧 | 历史记录 | 右侧面板 | 查看所有提交 |
| 底部 | 状态栏 | 最底部 | 显示推送/拉取状态 |

### 第三步：做第一次提交

1. 在你的项目文件夹里修改一些文件
2. 回到 GitHub Desktop，左侧「更改」面板会显示所有改动的文件
3. 在左下角的摘要框（Summary）输入提交说明，比如 "第一次提交"
4. 点击 `Commit to main`（提交到 main 分支）按钮
5. 点击顶部的 `Push origin`（推送）按钮，代码就上传到 GitHub 了

---

## 基本操作

### 克隆远程仓库

1. 点击 `File` → `Clone Repository`（文件 → 克隆仓库）
2. 选择你要克隆的仓库
3. 选择本地保存路径
4. 点击 `Clone`（克隆）

### 提交更改

1. 修改文件后，GitHub Desktop 左侧会列出所有改动
2. 每个文件前面有勾选框，可以选择要提交哪些文件
3. 在 `Summary`（摘要）框输入简短的提交说明（必填）
4. 在 `Description`（描述）框可以补充详细说明（可选）
5. 点击 `Commit to 当前分支名` 按钮

### 推送到远程

- 提交后，如果有未推送的更改，顶部会出现 `Push origin`（推送）按钮
- 点击即可将本地提交上传到 GitHub
- 按钮变成 `Fetch origin`（获取）表示已是最新

### 拉取最新代码

1. 点击 `Repository` → `Pull`（仓库 → 拉取）
2. 或者点击顶部的 `Fetch origin`，然后如果有新提交会显示 `Pull origin`
3. 拉取后本地代码就是远程最新的了

### 查看改动差异

在左侧「更改」面板中，点击任意文件，右侧会显示：
- 绿色行 = 新增的代码
- 红色行 = 删除的代码

---

## 分支管理

### 新建分支

1. 点击 `Branch` → `New Branch`（分支 → 新建分支）
2. 输入分支名称（建议用英文，如 `feature/login`）
3. 选择从哪个分支创建（一般选 main）
4. 点击 `Create branch`（创建分支）

### 切换分支

- 点击左上角分支名称旁边的下拉箭头
- 选择要切换的分支
- GitHub Desktop 会自动切换并更新文件

### 合并分支

1. 先切换到你要合并到的目标分支（比如 main）
2. 点击 `Branch` → `Merge Branch into Current`（分支 → 合并分支到当前分支）
3. 选择要合并的分支
4. 点击 `Merge <分支名> into <当前分支名>`
5. 如果没有冲突，合并完成
6. 点击 `Push origin` 推送到远程

### 解决冲突

如果合并时出现冲突：

1. GitHub Desktop 会提示合并冲突
2. 点击 `Open in Visual Studio Code`（在 VS Code 中打开）
3. 在 VS Code 中编辑冲突文件，选择保留哪些代码
4. 保存后回到 GitHub Desktop
5. 点击 `Commit merge`（提交合并）

---

## 常见问题

### Q: GitHub Desktop 有中文版吗？

A: 目前 GitHub Desktop 官方只提供英文界面，没有中文语言包。本指南通过翻译对照帮助你使用。

### Q: 如何修改仓库保存位置？

A: 点击 `File` → `Options`（文件 → 选项），在 `Accounts`（账号）或 `Git` 设置中可以修改本地仓库路径。

### Q: 提交时提示 "Author identity unknown"？

A: 需要配置 Git 用户信息。点击 `File` → `Options` → `Git`（文件 → 选项 → Git），输入你的姓名和邮箱。

### Q: 如何撤销最近一次提交？

A: 点击 `History`（历史），右键点击最近一次提交，选择 `Undo Commit`（撤销提交）。注意：这会把改动放回工作区，不会删除文件。

### Q: Push 失败怎么办？

A: 通常是因为远程有新的提交。先点击 `Fetch origin` → `Pull origin` 拉取最新代码，解决冲突后再 Push。

---

## 许可证

本仓库内容仅供学习参考。GitHub Desktop 版权归 GitHub, Inc. 所有。
