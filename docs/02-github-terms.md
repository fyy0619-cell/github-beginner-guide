## 2. GitHub 常见页面和术语

### 2.1 Repository / Repo / 仓库

**仓库就是一个项目的存放空间。**

一个仓库通常包含：

- 项目代码
- README 说明文档
- 配置文件
- 图片、脚本、测试文件
- 提交历史
- 分支
- Issue 和 Pull Request

例如：你做一个计算器项目，就可以建一个仓库叫 `calculator`。

### 2.2 Star

**Star 类似收藏/点赞。**

作用：

- 表示你喜欢这个项目。
- 以后可以在自己的 Star 列表里找到它。
- Star 越多，通常代表项目越受欢迎，但不代表一定适合你。

### 2.3 Fork

**Fork 是把别人的仓库复制一份到你的账号下。**

一句话理解：

```text
别人的仓库 -> Fork -> 你的 GitHub 账号下出现一个副本
```

#### Fork 为什么要这样操作？

因为你通常不能直接修改别人的仓库。Fork 的作用是先复制一份到你自己的账号下，你可以在自己的副本里随便改，不会影响原作者的项目。

Fork 常见用途：

- **学习代码**：把优秀项目 Fork 到自己账号下，慢慢研究。
- **二次开发**：基于别人的项目做自己的版本。
- **贡献开源**：修改后通过 Pull Request 请求原作者合并。
- **保存副本**：担心原项目以后删除，可以保留一份副本。

#### Fork 在哪里操作？

Fork 是 **GitHub 网页端操作**，不是本地终端命令。

操作步骤：

1. 打开别人的 GitHub 仓库页面。
2. 点击右上角 `Fork` 按钮。
3. 选择你的账号作为 Owner。
4. Repository name 可以保持原名，也可以改名。
5. 点击 `Create fork`。
6. 创建完成后，你会跳转到你自己账号下的新仓库。

例如：

```text
原仓库：https://github.com/original-owner/demo
Fork 后：https://github.com/your-name/demo
```

#### Fork 后通常还要做什么？

如果你只是在线查看，可以停在网页端。

如果你要在电脑上修改代码，还需要 **Clone 到本地**：

```bash
git clone https://github.com/你的用户名/仓库名.git
```

然后进入项目目录：

```bash
cd 仓库名
```

#### Fork、Clone、Download ZIP 的区别

| 操作 | 在哪里操作 | 得到什么 | 适合什么情况 |
| --- | --- | --- | --- |
| Fork | GitHub 网页端 | 你账号下的远程副本 | 想改别人的项目，或想给别人提交 PR |
| Clone | 本地终端 | 电脑上的完整 Git 仓库 | 想在本地开发、提交、同步更新 |
| Download ZIP | GitHub 网页端 | 一个普通压缩包 | 只想看代码或拿文件，不需要 Git 历史 |

Fork 之后，原仓库不会被你直接改动，你是在自己的副本里修改。
### 2.4 Clone

**Clone 是把远程仓库下载到你的电脑。**

例如：

```bash
git clone https://github.com/用户名/仓库名.git
```

Clone 后，你的电脑上会出现一个项目文件夹。

### 2.5 Commit

**Commit 是一次保存记录。**

每次 Commit 都应该说明你做了什么，例如：

```text
Add login page
Fix button style
Update README
```

新手可以理解为“给当前项目拍一张快照”。

### 2.6 Branch / 分支

**分支是独立开发线。**

常见分支：

- `main`：主分支，通常存放稳定代码。
- `dev`：开发分支。
- `feature/login`：某个具体功能分支。

使用分支可以避免直接把主分支搞坏。

### 2.7 Pull Request / PR

**PR 是请求把一个分支的代码合并到另一个分支。**

常见场景：

- 你 Fork 了别人项目，改完后向原项目发 PR。
- 团队成员在功能分支开发，完成后向 `main` 发 PR。

PR 页面可以讨论代码、审查修改、运行测试、最终合并。

### 2.8 Issue

**Issue 是问题、需求、任务的讨论区。**

可以用来：

- 报告 Bug。
- 提出新功能建议。
- 记录待办任务。
- 讨论项目计划。

### 2.9 Release

**Release 是项目的正式发布版本。**

比如：

```text
v1.0.0 第一个稳定版
v1.1.0 增加新功能
v1.1.1 修复 Bug
```

### 2.10 Actions

**GitHub Actions 是自动化工具。**

它可以自动：

- 运行测试。
- 构建项目。
- 发布网站。
- 打包软件。
- 检查代码格式。

---

---

[上一章：Git 和 GitHub 到底是什么？](01-git-vs-github.md) | [返回首页](../README.md) | [下一章：一个 GitHub 仓库通常由哪些部分组成？](03-repository-structure.md)
