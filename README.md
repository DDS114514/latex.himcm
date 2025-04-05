# 项目规范

欢迎使用本项目！下面是简单易懂的指南，帮助你快速上手。

---

## 1. 克隆项目 & 自动暂存配置

### 克隆项目
在终端（Terminal）输入下面的命令，把项目下载到你的电脑：
```bash
git clone https://github.com/yourusername/MathModelingProject.git
```

### 配置自动暂存（auto-stash）
为避免在拉取代码（pull）时出现未保存的修改，请设置自动暂存：
```bash
git config --global rebase.autoStash true
```
这会自动把你本地的修改暂时保存，再合并最新代码后恢复它们。

---

## 2. 上传更新流程

假设你已经修改了项目文件，按照以下步骤操作（假设没有冲突）：

1. **拉取最新代码**
   ```bash
   git pull origin main
   ```
2. **添加修改文件**
   ```bash
   git add .
   ```
3. **提交修改**
   ```bash
   git commit -m "简短说明：例如更新了介绍部分"
   ```
4. **推送到远程仓库**
   ```bash
   git push origin main
   ```

**示例流程：**
```bash
# 1. 拉取最新代码
git pull origin main

# 2. 添加修改（假设修改了 introduction.tex）
git add sections/introduction.tex

# 3. 提交修改
git commit -m "更新介绍部分的背景描述"

# 4. 推送更新
git push origin main
```

---

## 3. 关于使用 LaTeX

- **README 文件**  
  我们的 README 文件用 Markdown 编写，GitHub 会自动显示。  
- **LaTeX 公式**  
  如果需要写数学公式，可以用美元符号包围，例如：  
  ```markdown
  例如：$E=mc^2$
  ```
- **详细文档**  
  更详细的 LaTeX 文档放在 \`paper/\` 目录下，里面有完整的论文内容和编译说明。

---

按照以上步骤操作，就能快速开始项目协作了！
