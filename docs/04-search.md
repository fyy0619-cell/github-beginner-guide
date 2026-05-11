## 4. 如何搜索自己想要的东西？

GitHub 搜索非常强大，学会搜索，你就能找到很多优秀项目。

### 4.1 最基础搜索

进入 GitHub 首页顶部搜索框，输入关键词，例如：

```text
vue admin
python crawler
react dashboard
stm32 bootloader
machine learning
```

回车后，可以切换搜索类型：

- Repositories：搜索仓库。
- Code：搜索代码。
- Issues：搜索问题。
- Pull requests：搜索 PR。
- Discussions：搜索讨论。
- Users：搜索用户。

### 4.2 搜索仓库

如果你想找项目，优先看 Repositories。

可以关注这些指标：

- Stars：收藏数，越多通常越受欢迎。
- Forks：复制数，越多说明很多人在改或用。
- Last updated：最近更新时间，太久没更新的项目要谨慎。
- README：说明是否清楚。
- Issues：问题是否有人维护。
- License：许可证是否允许你使用。

### 4.3 常用搜索语法

#### 按语言搜索

```text
language:Python crawler
language:JavaScript dashboard
language:C bootloader
language:C++ game engine
```

#### 按 Star 数搜索

```text
stars:>1000 react admin
stars:>500 python spider
```

#### 按更新时间搜索

```text
pushed:>2025-01-01 vue3 admin
```

表示搜索 2025 年 1 月 1 日之后还更新过的项目。

#### 按仓库名搜索

```text
in:name blog
in:name dashboard
```

#### 按 README 搜索

```text
in:readme tutorial github
in:readme stm32
```

#### 按描述搜索

```text
in:description low code
in:description open source erp
```

#### 组合搜索

```text
vue3 admin language:TypeScript stars:>1000 pushed:>2025-01-01
python fastapi template stars:>500 pushed:>2025-01-01
stm32 bootloader language:C stars:>100
```

### 4.4 搜索代码

如果你想找某段代码怎么写，可以切换到 Code。

示例：

```text
filename:package.json vite react
filename:CMakeLists.txt stm32
extension:py requests beautifulsoup
```

常用语法：

```text
filename:文件名
extension:扩展名
path:目录
repo:用户名/仓库名
```

例如：

```text
repo:microsoft/vscode filename:package.json
```

### 4.5 如何判断一个项目值不值得学？

建议按这个顺序看：

1. README 是否清楚。
2. 最近是否还在维护。
3. Star 和 Fork 是否比较多。
4. Issues 是否有人回复。
5. 是否有安装和运行步骤。
6. 是否有 License。
7. 代码结构是否清晰。

不要只看 Star。一个项目 Star 很高，但多年不维护，也可能不适合新项目使用。

---

---

[上一章：一个 GitHub 仓库通常由哪些部分组成？](03-repository-structure.md) | [返回首页](../README.md) | [下一章：如何一步步新建自己的 GitHub 仓库？](05-create-repository.md)
