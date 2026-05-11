# GitHub 零基础完整入门指南

> 目标：让完全没用过 GitHub 的新手，能看懂 GitHub 是什么、怎么搜索项目、怎么新建仓库、怎么上传代码、怎么协作、怎么使用常见 Git 指令。

这个仓库已经按章节拆分成 `docs/` 目录。你在 GitHub 仓库左侧文件列表里点开 `docs`，就能像看目录一样按章节阅读。

## 推荐阅读顺序

| 顺序 | 章节 | 你会学到什么 |
| --- | --- | --- |
| 0 | [先看懂 GitHub 的整体流程图](docs/00-overview.md) | 先用流程图建立整体概念 |
| 1 | [Git 和 GitHub 到底是什么](docs/01-git-vs-github.md) | 区分 Git 工具和 GitHub 网站 |
| 2 | [GitHub 常见页面和术语](docs/02-github-terms.md) | Repository、Star、Fork、Clone、PR、Issue |
| 3 | [GitHub 仓库组成部分](docs/03-repository-structure.md) | README、LICENSE、.gitignore、Issues、Actions |
| 4 | [如何搜索自己想要的东西](docs/04-search.md) | 搜索项目、代码、文档和筛选优质项目 |
| 5 | [如何一步步新建自己的 GitHub 仓库](docs/05-create-repository.md) | 网页端创建仓库的完整步骤 |
| 6 | [如何把本地项目上传到 GitHub](docs/06-upload-local-project.md) | 本地终端上传代码到 GitHub |
| 7 | [如何下载别人项目、文档和 Fork 贡献](docs/07-download-and-fork.md) | Download ZIP、Clone、Fork、PR、同步 Fork |
| 8 | [哪些在网页端操作，哪些在本地终端操作](docs/08-web-vs-terminal.md) | 明确每一步到底在哪里做 |
| 9 | [Git 常用指令大全](docs/09-git-commands.md) | 常用 Git 命令速查 |
| 10 | [一个标准开发流程](docs/10-standard-workflow.md) | 个人开发和多人协作流程 |
| 11 | [Markdown 基础语法](docs/11-markdown-basics.md) | 写 README 必备语法 |
| 12 | [新手常见问题](docs/12-faq.md) | push 失败、main/master、大文件、密码等 |
| 13 | [推荐新手练习路线](docs/13-practice-roadmap.md) | 5 天练习路线 |
| 14 | [建议你记住的最小命令集](docs/14-minimum-commands.md) | 新手先背这些命令就够了 |
| 15 | [从零上传本仓库到你的 GitHub](docs/15-upload-this-repo.md) | 把这个教程仓库推到你的账号下 |
| 16 | [最后一句话](docs/16-final-summary.md) | GitHub 核心心法总结 |

## 仓库结构

```text
github-beginner-guide/
├── README.md                  # 首页导航
├── LICENSE                    # 开源许可证
├── .gitignore                 # Git 忽略规则
└── docs/                      # 分章节教程目录
    ├── README.md              # docs 目录索引
    ├── 00-overview.md
    ├── 01-git-vs-github.md
    ├── 02-github-terms.md
    ├── 03-repository-structure.md
    ├── 04-search.md
    ├── 05-create-repository.md
    ├── 06-upload-local-project.md
    ├── 07-download-and-fork.md
    ├── 08-web-vs-terminal.md
    ├── 09-git-commands.md
    ├── 10-standard-workflow.md
    ├── 11-markdown-basics.md
    ├── 12-faq.md
    ├── 13-practice-roadmap.md
    ├── 14-minimum-commands.md
    ├── 15-upload-this-repo.md
    └── 16-final-summary.md
```

## 新手怎么读最舒服？

1. 先打开 [流程图章节](docs/00-overview.md)，不要急着背命令。
2. 再看 [网页端和本地终端区别](docs/08-web-vs-terminal.md)，弄清楚每一步在哪里操作。
3. 如果你想建自己的仓库，看 [新建仓库](docs/05-create-repository.md) 和 [上传本地项目](docs/06-upload-local-project.md)。
4. 如果你想下载别人项目，看 [下载、Fork 和贡献](docs/07-download-and-fork.md)。
5. 平时忘记命令时，直接查 [Git 常用指令大全](docs/09-git-commands.md)。

## 一句话总结

```text
GitHub 网页端负责：创建、查看、讨论、合并
本地电脑终端负责：下载、修改、提交、推送
```
