# 新手上路：从安装到第一次推送

本文手把手教你从零开始使用 GitHub Desktop。

## 一、下载安装

1. 打开官网：https://desktop.github.com/
2. 点击下载按钮，下载 Windows 版本
3. 双击安装包，等待安装完成
4. 启动 GitHub Desktop

## 二、登录账号

1. 第一次打开会提示登录
2. 点击 `Sign in to GitHub.com`（登录 GitHub.com）
3. 浏览器会自动打开授权页面
4. 点击 `Authorize desktop`（授权）
5. 回到 GitHub Desktop，登录成功

> 如果你还没有 GitHub 账号，先去 https://github.com/signup 注册一个。

## 三、创建第一个仓库

### 方式一：创建教程仓库（推荐新手）

1. 在欢迎页点击 `Create a tutorial repository...`（创建一个教程仓库）
2. GitHub Desktop 会自动：
   - 在你本地创建一个练习文件夹
   - 生成一个 README 文件
   - 做第一次提交
3. 跟着提示一步步操作，学会基本流程

### 方式二：手动新建仓库

1. 点击 `File` → `New Repository`（文件 → 新建仓库）
2. 填写信息：
   - **Name（名称）**：仓库名，比如 `my-first-project`
   - **Description（描述）**：简单描述这个项目是做什么的
   - **Local path（本地路径）**：选择保存在电脑哪个位置
   - **Git ignore**：选择你用的编程语言（没有就选 None）
   - **License**：选择开源协议（新手选 MIT 就行）
3. 点击 `Create repository`（创建仓库）

## 四、认识主界面

创建仓库后，你会看到这样的界面：

```
┌─────────────────────────────────────────────────┐
│ File Edit View Repository Branch Help           │
├──────┬──────────────────────┬───────────────────┤
│ 当前  │                      │                   │
│ 仓库  │   更改（Changes）    │   历史（History）  │
│ 分支  │                      │                   │
│      │   修改的文件列表      │   提交记录列表     │
│      │                      │                   │
│      │   摘要: [________]   │   每次提交一行     │
│      │   描述: [________]   │                   │
│      │   [提交到 main]      │                   │
├──────┴──────────────────────┴───────────────────┤
│  底部状态栏：主分支 | 获取/推送 状态              │
└─────────────────────────────────────────────────┘
```

## 五、做第一次提交

### 1. 修改文件

1. 点击 `Repository` → `Open in Explorer`（仓库 → 在资源管理器中打开）
2. 你会看到仓库文件夹里有一个 `README.md` 文件
3. 用记事本或 VS Code 打开它，写点内容，比如：
   ```
   我的第一个 GitHub 项目
   ====================
   这是我用 GitHub Desktop 管理的第一个项目。
   ```
4. 保存文件

### 2. 回到 GitHub Desktop

你会看到左侧「更改」面板里出现了 `README.md`，前面有个绿色圆点，表示这个文件被修改了。

### 3. 写提交说明

- **Summary（摘要）**：必填，写一句话说明这次改了什么，比如 "更新了 README"
- **Description（描述）**：选填，可以写更详细的说明

### 4. 提交

点击蓝色按钮 `Commit to main`（提交到 main）。

提交后，左侧「更改」面板变空，右侧「历史」面板里出现了你刚做的提交。

## 六、推送到 GitHub

现在代码还只在你电脑上，要推送到 GitHub 网站：

1. 点击顶部的 `Publish repository`（发布仓库）按钮
2. 在弹出的窗口中：
   - 确认仓库名称
   - 填写描述
   - 勾选 `Keep this code private`（保持私有）如果不想公开
3. 点击 `Publish repository`

推送成功后：
- 按钮变成 `Fetch origin`（获取）
- 你可以去 https://github.com/你的用户名/仓库名 看到你的代码

## 七、日常工作流程

以后每天的开发流程就是这三步：

```
修改文件 → 提交（Commit） → 推送（Push）
```

需要同步别人的代码时：

```
拉取（Pull） ← 别人推送了新代码
```

## 八、打开项目文件夹

在 GitHub Desktop 中随时可以打开项目文件夹：

- 点击菜单 `Repository` → `Open in Explorer`（仓库 → 在资源管理器中打开）
- 或者右键点击仓库名 → `Open in Explorer`

## 九、用 VS Code 编辑代码

推荐把 GitHub Desktop 和 VS Code 配合使用：

1. 点击 `File` → `Options`（文件 → 选项）
2. 找到 `Integrations`（集成）或 `External Editor`（外部编辑器）
3. 选择 `Visual Studio Code`
4. 之后在 GitHub Desktop 中右键文件就能直接用 VS Code 打开
