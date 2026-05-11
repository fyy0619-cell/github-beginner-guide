## 7.7 哪些在网页端操作？哪些在本地终端操作？

这是新手最容易混的地方。记住一句话：

```text
GitHub 网页端负责：创建、查看、讨论、合并
本地电脑终端负责：下载、修改、提交、推送
```

### 网页端操作清单

这些操作一般在浏览器里的 GitHub 网站完成：

| 操作 | 在哪里点 | 为什么在网页端做 |
| --- | --- | --- |
| 注册/登录账号 | github.com | 账号属于 GitHub 网站 |
| 搜索项目 | 顶部搜索框 | GitHub 收录了所有公开仓库 |
| Star 收藏项目 | 仓库右上角 Star | 这是 GitHub 账号行为 |
| Fork 别人项目 | 仓库右上角 Fork | 复制远程仓库到你的账号下 |
| 新建仓库 | 右上角 `+` 或左侧 `New` | 远程仓库创建在 GitHub 服务器上 |
| 查看 README | 仓库首页 | GitHub 自动渲染 Markdown |
| 提 Issue | `Issues` 标签页 | 问题讨论发生在项目页面 |
| 创建 Pull Request | `Pull requests` 标签页 | 请求合并代码需要在 GitHub 上审查 |
| 合并 Pull Request | PR 页面 `Merge` 按钮 | 合并远程分支由 GitHub 执行 |
| 下载 ZIP | `Code -> Download ZIP` | 浏览器直接下载压缩包 |
| 同步 Fork | `Sync fork` | GitHub 可以在线同步原仓库更新 |

### 本地终端操作清单

这些操作一般在你电脑上的 PowerShell、CMD、Git Bash 或 VS Code 终端里完成：

| 命令 | 在哪里执行 | 作用 |
| --- | --- | --- |
| `git config` | 本地终端 | 配置你的 Git 用户名和邮箱 |
| `git clone` | 本地终端 | 把 GitHub 仓库下载到电脑 |
| `cd 项目目录` | 本地终端 | 进入项目文件夹 |
| `git init` | 本地终端 | 把普通文件夹变成 Git 仓库 |
| `git status` | 本地终端 | 查看哪些文件被修改 |
| `git diff` | 本地终端 | 查看文件具体改了什么 |
| `git add .` | 本地终端 | 把修改加入暂存区 |
| `git commit -m "说明"` | 本地终端 | 保存一个本地版本 |
| `git remote add origin 地址` | 本地终端 | 关联 GitHub 远程仓库 |
| `git push` | 本地终端 | 把本地提交上传到 GitHub |
| `git pull` | 本地终端 | 把 GitHub 最新内容拉到本地 |
| `git switch -c 分支名` | 本地终端 | 新建并切换分支 |
| `git merge 分支名` | 本地终端 | 合并本地分支 |

### 最常见的混合流程

很多 GitHub 操作是“网页端 + 本地终端”配合完成的。

#### 上传自己的新项目

```text
网页端：New repository 创建空仓库
本地终端：git init -> git add -> git commit -> git remote -> git push
网页端：刷新仓库页面，检查代码是否上传成功
```

#### 下载并运行别人的项目

```text
网页端：打开仓库，复制 Code 里的 HTTPS 地址
本地终端：git clone 地址
本地终端：进入项目并按照 README 安装运行
```

#### 给别人项目贡献代码

```text
网页端：Fork 原项目
本地终端：git clone 你的 Fork
本地终端：新建分支、修改、commit、push
网页端：创建 Pull Request
网页端：根据作者反馈继续修改或等待合并
```

#### 只下载文档

```text
网页端：直接看 README 或 docs
网页端：需要保存时点击 Raw 后另存为
网页端：需要全部文档时 Download ZIP
```

### 判断一个操作在哪里做的小技巧

- 要点按钮、看页面、写评论、创建 PR：通常在 **GitHub 网页端**。
- 要操作电脑里的文件、提交版本、上传下载代码：通常在 **本地终端**。
- 要写代码或改文档：通常在 **代码编辑器**，比如 VS Code。
- 要把本地改动同步到 GitHub：最后一定会用到 **`git push`**。
- 要把 GitHub 上的新内容同步到本地：通常用 **`git pull`**。

---

---

[上一章：如何从 GitHub 下载别人的项目和文档？](07-download-and-fork.md) | [返回首页](../README.md) | [下一章：Git 常用指令大全](09-git-commands.md)
