## 3. 一个 GitHub 仓库通常由哪些部分组成？

打开一个仓库，你通常会看到这些部分。

### 3.1 Code

**Code 是仓库首页和文件列表。**

你可以在这里：

- 查看代码文件。
- 查看目录结构。
- 下载 ZIP。
- Clone 仓库。
- 切换分支。
- 查看最近提交。

### 3.2 README.md

**README 是项目说明书，通常是仓库最重要的文档。**

一个好的 README 应该说明：

- 项目是做什么的。
- 项目有什么功能。
- 如何安装。
- 如何运行。
- 如何使用。
- 项目目录结构。
- 常见问题。
- 作者和许可证。

`README.md` 使用 Markdown 语法编写。

### 3.3 LICENSE

**LICENSE 是开源许可证。**

它说明别人能不能使用、修改、分发你的项目。

常见许可证：

- MIT：非常宽松，适合大多数个人项目。
- Apache-2.0：宽松，并带有专利授权条款。
- GPL：要求衍生项目也开源。
- No license：没有许可证时，别人默认没有明确授权，不建议随便使用。

### 3.4 .gitignore

**.gitignore 用来告诉 Git 哪些文件不要上传。**

常见不上传的内容：

- 编译产物，如 `dist/`、`build/`。
- 依赖目录，如 `node_modules/`。
- 临时文件，如 `.DS_Store`。
- 密码、密钥、环境变量文件，如 `.env`。

示例：

```gitignore
node_modules/
dist/
.env
*.log
```

### 3.5 docs/

**docs 通常用来放文档。**

例如：

```text
docs/installation.md
docs/api.md
docs/faq.md
```

### 3.6 src/

**src 通常用来放源代码。**

例如：

```text
src/main.py
src/app.js
src/index.cpp
```

### 3.7 tests/

**tests 通常用来放测试代码。**

测试可以帮你检查代码是否正常工作。

### 3.8 Issues

**Issues 是项目问题列表。**

常见标签：

- `bug`：缺陷。
- `enhancement`：功能增强。
- `documentation`：文档问题。
- `good first issue`：适合新手贡献的问题。

### 3.9 Pull requests

**Pull requests 是代码合并请求列表。**

团队协作时，一般不是直接改 `main`，而是：

```text
新建分支 -> 修改代码 -> 提交 -> 发 PR -> 审查 -> 合并
```

### 3.10 Discussions

**Discussions 是讨论区。**

适合问答、想法交流、路线图讨论，不一定是明确 Bug。

### 3.11 Wiki

**Wiki 是项目知识库。**

适合放大量教程、设计说明、常见问题。

### 3.12 Projects

**Projects 是项目管理看板。**

可以像看板一样管理任务：

```text
To do -> In progress -> Done
```

### 3.13 Security

**Security 是安全相关页面。**

可以查看：

- 安全策略。
- 依赖漏洞提醒。
- 私密报告漏洞的入口。

### 3.14 Insights

**Insights 是仓库数据统计。**

可以查看：

- 提交活跃度。
- 贡献者。
- 流量。
- Fork 和 Star 趋势。

---

---

[上一章：GitHub 常见页面和术语](02-github-terms.md) | [返回首页](../README.md) | [下一章：如何搜索自己想要的东西？](04-search.md)
