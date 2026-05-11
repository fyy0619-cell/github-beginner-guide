## 7. 如何从 GitHub 下载别人的项目和文档？

下载之前先想清楚：你是只想看一眼，还是要长期学习和修改？不同目的对应不同方法。

### 7.1 三种下载方式怎么选？

| 目的 | 推荐方式 | 操作位置 | 是否保留 Git 历史 | 是否方便更新 |
| --- | --- | --- | --- | --- |
| 只想下载整个项目看一看 | Download ZIP | GitHub 网页端 | 否 | 不方便 |
| 想在本地运行、学习、修改 | git clone | 本地终端 | 是 | 方便 |
| 想修改后贡献给原作者 | Fork + Clone + PR | 网页端 + 本地终端 | 是 | 方便 |
| 只想下载某个单独文件 | Raw / Download raw file | GitHub 网页端 | 否 | 不方便 |
| 只想看项目文档 | 直接看 README / docs | GitHub 网页端 | 不涉及 | 不涉及 |

### 7.2 下载整个工程项目：Download ZIP

这是最简单的方法，不需要安装 Git。

**操作位置：GitHub 网页端。**

步骤：

1. 打开你想下载的 GitHub 仓库。
2. 点击绿色 `Code` 按钮。
3. 点击 `Download ZIP`。
4. 等待浏览器下载压缩包。
5. 解压 ZIP 文件。
6. 打开解压后的文件夹查看或运行项目。

适合：

- 只想快速看代码。
- 只想下载项目里的图片、文档、示例文件。
- 不准备提交修改。

不适合：

- 想长期跟踪项目更新。
- 想给项目提交 Pull Request。
- 想学习 Git 提交历史。

注意：ZIP 下载只是普通文件夹，没有 `.git` 历史，不能直接 `git pull` 更新。

### 7.3 下载完整工程项目：git clone

`git clone` 会把整个远程仓库复制到你的电脑，包括代码和 Git 提交历史。

**操作位置：本地电脑终端。**

步骤：

1. 打开别人的 GitHub 仓库页面。
2. 点击绿色 `Code` 按钮。
3. 复制 HTTPS 地址，例如：

```text
https://github.com/octocat/Hello-World.git
```

4. 在电脑上打开 PowerShell、CMD、Git Bash 或 VS Code 终端。
5. 进入你想保存项目的目录，例如：

```powershell
cd D:\projects
```

6. 执行 clone：

```bash
git clone https://github.com/octocat/Hello-World.git
```

7. 进入项目：

```bash
cd Hello-World
```

8. 查看文件：

```bash
dir        # Windows PowerShell/CMD
ls         # Git Bash / macOS / Linux
```

适合：

- 想在本地运行别人的项目。
- 想学习项目完整结构。
- 想以后用 `git pull` 拉取更新。
- 想查看提交历史。

更新别人项目的最新代码：

```bash
git pull
```

### 7.4 下载别人的文档

GitHub 项目文档常见位置：

```text
README.md              # 仓库首页说明
docs/                  # 文档目录
wiki                   # GitHub Wiki 页面
examples/              # 示例代码和示例文档
CHANGELOG.md           # 更新日志
CONTRIBUTING.md        # 贡献指南
```

#### 方法一：直接在网页端看文档

**操作位置：GitHub 网页端。**

步骤：

1. 打开仓库页面。
2. 先看首页自动显示的 `README.md`。
3. 如果有 `docs` 文件夹，点击进入。
4. 如果页面上方有 `Wiki`，点击查看 Wiki 文档。
5. 如果 README 里有目录链接，点击跳转到对应文档。

适合：只想阅读，不需要保存到电脑。

#### 方法二：下载单个文档文件

**操作位置：GitHub 网页端。**

步骤：

1. 打开某个 `.md`、`.txt`、`.pdf` 或代码文件。
2. 点击右上角的 `Raw` 或下载按钮。
3. 浏览器打开原始文件后，右键选择另存为。

适合：只想保存某一个文档。

#### 方法三：下载整个仓库里的全部文档

**操作位置：网页端或本地终端。**

如果不懂 Git，用 ZIP：

```text
Code -> Download ZIP -> 解压 -> 找 README.md 或 docs 文件夹
```

如果会 Git，用 clone：

```bash
git clone https://github.com/用户名/仓库名.git
```

然后在本地打开：

```text
README.md
docs/
```

### 7.5 Fork 别人项目并修改贡献

这是参与开源项目最常见的流程。

#### 第一步：Fork 原项目

**操作位置：GitHub 网页端。**

1. 打开原项目仓库。
2. 点击右上角 `Fork`。
3. 选择你的账号。
4. 点击 `Create fork`。

为什么要做这一步：你没有权限直接改原作者仓库，所以先复制一份到你账号下。

#### 第二步：Clone 你自己的 Fork

**操作位置：本地电脑终端。**

注意：这里 clone 的是你自己的 Fork，不是原作者仓库。

```bash
git clone https://github.com/你的用户名/仓库名.git
cd 仓库名
```

#### 第三步：新建分支再修改

**操作位置：本地电脑终端。**

```bash
git switch -c fix-typo
```

为什么要新建分支：不要直接在 `main` 上乱改，分支能让一次修改更清晰，也方便提交 PR。

#### 第四步：修改文件并提交

**操作位置：本地电脑终端 + 代码编辑器。**

```bash
git status
git add .
git commit -m "Fix typo in README"
```

#### 第五步：推送你的分支

**操作位置：本地电脑终端。**

```bash
git push -u origin fix-typo
```

#### 第六步：创建 Pull Request

**操作位置：GitHub 网页端。**

1. 打开你 Fork 后的仓库页面。
2. GitHub 通常会提示 `Compare & pull request`。
3. 点击它。
4. 确认方向是：

```text
你的分支 -> 原作者仓库的 main 分支
```

5. 写清楚你改了什么、为什么改。
6. 点击 `Create pull request`。

#### 第七步：等待作者审查

**操作位置：GitHub 网页端。**

作者可能会：

- 直接合并你的 PR。
- 评论让你继续修改。
- 关闭 PR。
- 暂时不处理。

如果作者让你修改，你继续在本地改，然后：

```bash
git add .
git commit -m "Update according to review"
git push
```

PR 页面会自动更新。

### 7.6 Fork 后如何同步原项目更新？

如果原作者项目更新了，你的 Fork 可能会落后。

#### 简单方法：网页端同步

**操作位置：GitHub 网页端。**

1. 打开你 Fork 后的仓库。
2. 如果看到 `Sync fork`，点击它。
3. 点击 `Update branch`。

#### 进阶方法：终端同步

**操作位置：本地电脑终端。**

第一次添加原仓库地址：

```bash
git remote add upstream https://github.com/原作者用户名/原仓库名.git
```

查看远程地址：

```bash
git remote -v
```

同步原仓库更新：

```bash
git switch main
git fetch upstream
git merge upstream/main
git push origin main
```

这里的含义：

- `origin`：你自己 Fork 的仓库。
- `upstream`：原作者的仓库。
- `fetch upstream`：把原作者更新拉下来。
- `merge upstream/main`：合并到你的本地 main。
- `push origin main`：推回你自己的 GitHub Fork。

---

---

[上一章：如何把本地项目上传到 GitHub？](06-upload-local-project.md) | [返回首页](../README.md) | [下一章：哪些在网页端操作，哪些在本地终端操作](08-web-vs-terminal.md)

