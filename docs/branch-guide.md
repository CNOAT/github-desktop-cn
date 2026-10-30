# 分支管理与协作

本文介绍如何用 GitHub Desktop 管理分支和团队协作。

## 一、什么是分支？

分支就像电影的"平行宇宙"：
- **main 分支**：正式版本，始终保持可用
- **功能分支**：在平行宇宙里开发新功能，搞砸了也不影响正式版
- **合并**：功能做好了，再把平行宇宙的成果合并回 main

## 二、新建分支

### 步骤

1. 点击菜单 `Branch` → `New Branch`（分支 → 新建分支）
2. 输入分支名称：
   - 建议用英文，比如 `feature/login-page`（登录页面功能）
   - 命名规范：`feature/功能名`、`bugfix/问题名`
3. 选择从哪个分支创建（一般选 `main`）
4. 点击 `Create branch`（创建分支）

### 注意

- 创建新分支后，你的所有提交都会在这个新分支上，不影响 main
- 左上角分支名会变成你刚创建的分支名

## 三、切换分支

### 方法一：下拉选择

1. 点击左上角分支名称旁边的下拉箭头
2. 在列表中选择要切换的分支
3. GitHub Desktop 会自动切换，项目文件夹里的文件也会跟着变

### 方法二：菜单

点击 `Branch` → 底部会列出所有分支，直接选择

## 四、在分支上开发

1. 确认左上角显示的是你的功能分支名
2. 正常修改文件、提交代码
3. 这些提交都在功能分支上，main 分支不受影响

## 五、推送分支到远程

新分支默认只在你本地。要推送到 GitHub：

1. 点击顶部的 `Publish branch`（发布分支）按钮
2. 推送后，其他人就能在 GitHub 上看到这个分支了

## 六、合并分支

功能开发完成后，要合并回 main：

### 步骤

1. **先切换到 main 分支**
   - 点击分支下拉框，选择 `main`
   - 点击 `Fetch origin` → `Pull origin`，确保 main 是最新的

2. **执行合并**
   - 点击菜单 `Branch` → `Merge Branch into Current`（分支 → 合并分支到当前分支）
   - 选择你要合并的功能分支，比如 `feature/login-page`
   - 点击 `Merge feature/login-page into main`

3. **推送**
   - 合并后点击 `Push origin` 推送到远程

## 七、删除已合并的分支

合并完成后，功能分支就没用了，可以删掉：

1. 切换到 main 分支
2. 点击菜单 `Branch` → `Delete Branch`（分支 → 删除分支）
3. 选择要删除的分支
4. 确认删除

> 删除前确保已经合并到 main，否则分支上的代码会丢失。

## 八、处理合并冲突

如果两个人改了同一个文件的同一行，合并时会冲突。

### 冲突提示

GitHub Desktop 会显示：
```
Unable to merge because of conflicts
```
（无法合并，存在冲突）

### 解决步骤

1. 点击 `Open in Visual Studio Code`（在 VS Code 中打开）
2. 在 VS Code 中找到冲突标记：
   ```
   <<<<<<< HEAD
   你写的代码
   =======
   别人写的代码
   >>>>>>> branch-name
   ```
3. 决定保留哪些代码，删掉冲突标记和不需要的代码
4. 保存文件
5. 回到 GitHub Desktop，点击 `Commit merge`（提交合并）
6. 点击 `Push origin` 推送

## 九、团队协作流程

多人协作的标准流程：

```
1. 每个人从 main 拉新分支
   git checkout -b feature/xxx

2. 在自己的分支上开发、提交、推送

3. 在 GitHub 上发起 Pull Request（合并请求）

4. 同事审查代码（Code Review）

5. 审查通过后，合并到 main

6. 所有人拉取最新的 main
```

### 在 GitHub Desktop 中发起 Pull Request

1. 推送分支后，点击 `Branch` → `Create Pull Request`（分支 → 创建合并请求）
2. 浏览器会打开 GitHub 的 PR 页面
3. 填写标题和说明，请求同事审查

## 十、常用分支操作速查

| 操作 | 菜单位置 |
|------|------|
| 新建分支 | Branch → New Branch |
| 切换分支 | 左上角分支下拉框 |
| 重命名分支 | Branch → Rename Branch |
| 删除分支 | Branch → Delete Branch |
| 合并分支 | Branch → Merge Branch into Current |
| 发布分支 | 顶部 Publish branch 按钮 |
| 比较分支差异 | Branch → Compare Branch to |
| 从 main 更新当前分支 | Branch → Update from main |
