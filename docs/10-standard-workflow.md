## 9. 一个标准开发流程

### 9.1 自己一个人开发

```bash
git status
git add .
git commit -m "Update feature"
git push
```

日常循环：

```text
修改文件 -> git status -> git add -> git commit -> git push
```

### 9.2 多人协作开发

推荐流程：

```text
1. 从 main 拉取最新代码
2. 新建功能分支
3. 在功能分支修改代码
4. 提交 commit
5. 推送分支到 GitHub
6. 创建 Pull Request
7. 代码审查
8. 合并到 main
```

对应指令：

```bash
git switch main
git pull
git switch -c feature/login
git add .
git commit -m "Add login feature"
git push -u origin feature/login
```

然后到 GitHub 页面创建 PR。

---

---

[上一章：Git 常用指令大全](09-git-commands.md) | [返回首页](../README.md) | [下一章：Markdown 基础语法](11-markdown-basics.md)
