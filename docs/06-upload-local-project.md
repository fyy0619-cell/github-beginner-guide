## 6. 如何把本地项目上传到 GitHub？

假设你已经在 GitHub 创建了空仓库：

```text
https://github.com/你的用户名/my-first-repo
```

### 6.1 第一次配置 Git 用户信息

只需要在电脑上配置一次：

```bash
git config --global user.name "你的 GitHub 用户名"
git config --global user.email "你的邮箱"
```

查看配置：

```bash
git config --global --list
```

### 6.2 进入你的项目目录

```bash
cd 你的项目目录
```

Windows 示例：

```powershell
cd D:\projects\my-first-repo
```

### 6.3 初始化 Git 仓库

```bash
git init
```

### 6.4 查看当前状态

```bash
git status
```

### 6.5 添加文件到暂存区

添加全部文件：

```bash
git add .
```

只添加某个文件：

```bash
git add README.md
```

### 6.6 提交版本

```bash
git commit -m "Initial commit"
```

### 6.7 设置主分支名为 main

```bash
git branch -M main
```

### 6.8 关联远程仓库

```bash
git remote add origin https://github.com/你的用户名/my-first-repo.git
```

查看远程地址：

```bash
git remote -v
```

### 6.9 推送到 GitHub

```bash
git push -u origin main
```

第一次推送可能要求登录 GitHub。

---

---

[上一章：如何一步步新建自己的 GitHub 仓库？](05-create-repository.md) | [返回首页](../README.md) | [下一章：如何从 GitHub 下载别人的项目和文档？](07-download-and-fork.md)
