## 11. 新手常见问题

### 11.1 为什么 push 失败？

常见原因：

- 没有登录 GitHub。
- 远程地址写错。
- 当前分支名不是 `main`。
- 远程仓库已经有内容，本地没有先 pull。
- 没有权限推送到别人的仓库。

排查：

```bash
git remote -v
git branch
git status
git pull --rebase origin main
git push
```

### 11.2 main 和 master 有什么区别？

它们都是分支名。

以前很多项目默认叫 `master`，现在 GitHub 默认叫 `main`。新项目建议使用 `main`。

### 11.3 能不能上传大文件？

不建议直接上传很大的文件。

GitHub 普通仓库对大文件有限制。大文件建议使用：

- Git LFS
- 云盘
- Release 附件
- 对象存储

### 11.4 能不能上传密码？

绝对不要上传密码、Token、私钥、`.env` 文件。

如果不小心上传了：

1. 立刻删除并提交。
2. 去对应平台重置密码或 Token。
3. 如果已经进入历史记录，需要进一步清理 Git 历史。

### 11.5 Public 和 Private 怎么选？

- 学习项目、作品集、开源项目：可以 Public。
- 商业项目、课程作业、含隐私内容：建议 Private。

---

---

[上一章：Markdown 基础语法](11-markdown-basics.md) | [返回首页](../README.md) | [下一章：推荐新手练习路线](13-practice-roadmap.md)
