## 0. 先看懂 GitHub 的整体流程图

如果你是第一次接触 GitHub，先不要急着背命令。先把下面几张图看懂，你就知道每一步在干什么。

### 0.1 GitHub 学习路线总览

```mermaid
flowchart TD
    A[注册并登录 GitHub] --> B[学会搜索项目]
    B --> C[看懂仓库页面]
    C --> D[新建自己的仓库]
    D --> E[在电脑上安装并配置 Git]
    E --> F[把本地项目上传到 GitHub]
    F --> G[日常修改代码并提交]
    G --> H[学习分支和 Pull Request]
    H --> I[参与开源或团队协作]
```

你可以把 GitHub 学习分成三层：

| 阶段 | 你要学会什么 | 关键动作 |
| --- | --- | --- |
| 入门 | 会找、会看、会收藏 | Search、README、Star |
| 上手 | 会建仓库、会上传 | New repository、commit、push |
| 进阶 | 会协作、会贡献 | Branch、Issue、Pull Request |

### 0.2 从网页新建仓库的流程图

```mermaid
flowchart TD
    A[打开 github.com 并登录] --> B[点击右上角 + 或左侧 New]
    B --> C[选择 New repository]
    C --> D[填写仓库名 Repository name]
    D --> E[填写描述 Description]
    E --> F{选择可见性}
    F --> G[Public 公开]
    F --> H[Private 私有]
    G --> I{是否初始化文件}
    H --> I
    I --> J[新手网页创建: 可勾选 README]
    I --> K[已有本地项目: 不要勾选 README]
    J --> L[点击 Create repository]
    K --> L
```

重点记住：

- 如果你准备从零在网页上写项目，可以勾选 README。
- 如果你本地已经有项目，要上传到 GitHub，通常不要勾选 README、.gitignore、License，避免第一次 push 冲突。

### 0.3 本地项目上传到 GitHub 的流程图

```mermaid
flowchart LR
    A[本地项目文件夹] --> B[git init 初始化]
    B --> C[git add . 加入暂存区]
    C --> D[git commit 保存版本]
    D --> E[git remote add origin 关联远程仓库]
    E --> F[git push 上传到 GitHub]
    F --> G[GitHub 仓库页面看到代码]
```

对应命令就是：

```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/你的用户名/仓库名.git
git push -u origin main
```

### 0.4 Git 日常工作流结构图

```mermaid
flowchart TD
    A[修改文件] --> B[git status 查看状态]
    B --> C[git diff 查看具体改动]
    C --> D[git add . 暂存改动]
    D --> E[git commit -m 写清楚提交说明]
    E --> F[git push 推送到 GitHub]
    F --> G[下一轮修改]
    G --> A
```

日常开发其实就是不断循环：

```text
修改 -> 查看 -> 添加 -> 提交 -> 推送
```

### 0.5 多人协作流程图

```mermaid
flowchart TD
    A[main 主分支保持稳定] --> B[从 main 新建功能分支]
    B --> C[在功能分支写代码]
    C --> D[提交 commit]
    D --> E[push 到 GitHub]
    E --> F[创建 Pull Request]
    F --> G[同伴审查代码]
    G --> H{是否需要修改}
    H -->|需要| C
    H -->|通过| I[合并到 main]
    I --> J[删除功能分支]
```

这个流程可以避免大家直接修改 `main`，也方便检查代码质量。

### 0.6 仓库组成结构图

```mermaid
flowchart TD
    A[一个 GitHub 仓库] --> B[Code 文件和目录]
    A --> C[README.md 项目说明]
    A --> D[LICENSE 开源许可证]
    A --> E[.gitignore 忽略文件规则]
    A --> F[Issues 问题和任务]
    A --> G[Pull Requests 合并请求]
    A --> H[Actions 自动化]
    A --> I[Projects 项目看板]
    A --> J[Wiki / docs 文档]
```

新手最先需要重点掌握这四个：

```text
Code：看代码在哪里
README.md：看项目怎么用
Issues：看别人遇到的问题
Pull Requests：看代码是怎么被合并的
```

---

---

[返回首页](../README.md) | [下一章：Git 和 GitHub 到底是什么？](01-git-vs-github.md)
