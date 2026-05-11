## 8. Git 常用指令大全

### 8.1 基础配置

```bash
git config --global user.name "你的名字"
git config --global user.email "你的邮箱"
git config --global --list
```

### 8.2 创建和查看仓库

```bash
git init                 # 初始化本地仓库
git status               # 查看当前状态
git log                  # 查看提交历史
git log --oneline        # 简洁查看提交历史
```

### 8.3 添加和提交

```bash
git add 文件名            # 添加指定文件
git add .                 # 添加全部修改
git commit -m "说明"      # 提交一次版本
```

### 8.4 分支操作

```bash
git branch                      # 查看本地分支
git branch 分支名                # 创建分支
git switch 分支名                # 切换分支
git switch -c 分支名             # 创建并切换分支
git merge 分支名                 # 合并指定分支到当前分支
git branch -d 分支名             # 删除本地分支
```

旧版 Git 也常用：

```bash
git checkout 分支名
git checkout -b 分支名
```

### 8.5 远程仓库操作

```bash
git remote -v                                      # 查看远程仓库
git remote add origin 仓库地址                      # 添加远程仓库
git push -u origin main                            # 第一次推送
git push                                           # 后续推送
git pull                                           # 拉取远程更新并合并
git fetch                                          # 只拉取，不自动合并
```

### 8.6 克隆仓库

```bash
git clone 仓库地址
```

### 8.7 撤销修改

撤销某个还没 add 的文件修改：

```bash
git restore 文件名
```

取消暂存：

```bash
git restore --staged 文件名
```

查看某个文件改了什么：

```bash
git diff 文件名
```

### 8.8 标签

```bash
git tag                         # 查看标签
git tag v1.0.0                  # 创建标签
git push origin v1.0.0          # 推送标签
git push origin --tags          # 推送所有标签
```

---

---

[上一章：哪些在网页端操作，哪些在本地终端操作](08-web-vs-terminal.md) | [返回首页](../README.md) | [下一章：一个标准开发流程](10-standard-workflow.md)

