## 14. 从零上传本仓库到你的 GitHub

如果你已经在 GitHub 创建了一个空仓库，比如：

```text
https://github.com/你的用户名/github-beginner-guide
```

在本目录执行：

```bash
git remote add origin https://github.com/你的用户名/github-beginner-guide.git
git branch -M main
git push -u origin main
```

如果提示远程仓库已有 README，可以先执行：

```bash
git pull --rebase origin main
git push -u origin main
```

---

---

[上一章：建议你记住的最小命令集](14-minimum-commands.md) | [返回首页](../README.md) | [下一章：最后一句话](16-final-summary.md)
