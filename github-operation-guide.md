# GitHub界面操作实战指南

这是一份专为从未使用过GitHub的新手准备的详细操作指南。我们将手把手教你如何在GitHub网站上提交你的第一个Issue。

## 🎯 开始之前

确保你已经：
- 注册了GitHub账号
- 能够正常访问GitHub网站
- 找到了你想要贡献的开源项目

## 📍 第一步：找到Issues入口

### 操作步骤
1. **打开项目主页**
   - 在浏览器中输入项目的GitHub地址，例如：`https://github.com/用户名/项目名`
   - 你会看到项目的代码仓库主页

2. **定位Issues标签页**
   - 在页面顶部，项目名称下方有一排导航标签
   - 从左到右你会看到：`<> Code`、`🔍 Issues`、`🔄 Pull requests` 等
   - **点击 `Issues` 标签页**

### 界面说明
```
用户名/项目名                                    Watch ⭐ Star 🍴 Fork
─────────────────────────────────────────────────────────────────
 📁 Code    🔍 Issues    🔄 Pull requests    📊 Actions    📝 Wiki
```

### 小提示
如果你看不到`Issues`标签，说明这个项目可能禁用了Issues功能，你需要联系项目维护者。

## 🔍 第二步：搜索现有Issues

在提交新Issue前，**必须先搜索**是否已有相似的问题。

### 操作步骤
1. **进入Issues页面后**，你会看到页面顶部有一个搜索框
2. **搜索框的默认内容**通常是 `is:issue is:open`
3. **在搜索框中输入关键词**，例如：
   - `登录失败`
   - `无法显示图片`
   - `安装错误`
   - `chrome 浏览器`

### 搜索技巧
- **使用具体的关键词**：不要只搜索"bug"或"问题"
- **尝试英文关键词**：如果是国际项目，也试试英文
- **查看已关闭的Issues**：在搜索框中改为 `is:issue is:closed 你的关键词`

### 界面说明
```
🔍 [is:issue is:open 你的搜索关键词]    Filters ▽    [New issue]

Issues列表：
─────────────────────────────────
🐛 登录页面显示异常 #123
   opened 2 days ago by user123
─────────────────────────────────
✨ 希望添加深色主题 #122
   opened 1 week ago by user456
```

## ➕ 第三步：创建新Issue

如果确认没有重复的Issue，开始创建新的。

### 操作步骤
1. **点击绿色的"New issue"按钮**
   - 这个按钮通常在Issues页面的右上角
   - 按钮颜色是GitHub的绿色主题色

2. **选择Issue模板（如果有）**
   - 一些项目会提供预设的模板选择页面
   - 常见的模板类型：
     - `🐛 Bug report` - 报告软件错误
     - `✨ Feature request` - 请求新功能
     - `📖 Documentation` - 文档相关
     - `❓ Question` - 提问求助
   - **选择最符合你情况的模板**，点击对应的"Get started"按钮

3. **如果没有模板**
   - 直接进入Issue编辑页面
   - 你需要按照我们提供的模板自行填写

## ✍️ 第四步：填写Issue内容

这是最重要的一步！一个好的Issue能大大提高被解决的可能性。

### 页面布局说明
Issue编辑页面分为几个主要区域：

```
标题栏: [在这里输入Issue标题]

内容编辑区域:
┌─ Write ─ Preview ─────────────────────────┐
│                                           │
│  在这里输入Issue的详细内容                │
│  支持Markdown语法                         │
│                                           │
│                                           │
└───────────────────────────────────────────┘

右侧边栏:
┌─ Assignees ────┐
├─ Labels ───────┤  ← 新手建议留空
├─ Projects ─────┤    让维护者处理
└─ Milestone ────┘
```

### 填写标题
**好的标题特征：**
- 简洁明了，一句话概括问题
- 包含关键信息
- 避免过于宽泛的词语

**标题示例：**
- ✅ "Chrome浏览器中登录按钮无响应"
- ✅ "上传大于10MB的文件时报错"
- ✅ "希望添加深色主题功能"
- ❌ "有问题"
- ❌ "这个不行"
- ❌ "请帮忙"

### 填写正文内容
**按照模板结构填写**，如果项目没有提供模板，可以参考我们的[标准模板](./issue-templates.md)。

**基本结构：**
1. **问题描述**：清楚说明遇到的问题
2. **重现步骤**：详细的操作步骤
3. **期望结果**：你认为应该发生什么
4. **实际结果**：实际发生了什么
5. **环境信息**：操作系统、浏览器、版本等

## 📝 Markdown基础语法

GitHub Issues支持Markdown语法，掌握基础语法能让你的Issue更清晰易读。

### 常用语法速查表

| 语法 | 效果 | 用途 |
|------|------|------|
| `# 标题` | # 大标题 | 主要标题 |
| `## 标题` | ## 中标题 | 小节标题 |
| `**粗体**` | **粗体** | 强调重点 |
| `*斜体*` | *斜体* | 轻微强调 |
| `` `代码` `` | `代码` | 行内代码 |
| `- 列表项` | • 列表项 | 无序列表 |
| `1. 列表项` | 1. 列表项 | 有序列表 |

### 代码块
当你需要贴代码或错误信息时：

````
```
你的代码或错误信息
放在这里
```
````

**指定编程语言（可选）：**
````
```javascript
console.log("Hello World");
```
````

### 插入图片
1. **直接拖拽**：将截图直接拖到编辑框中
2. **复制粘贴**：截图后直接Ctrl+V粘贴
3. **手动上传**：点击编辑框下方的"选择文件"

### 提及用户
使用 `@用户名` 可以通知特定用户：
```
@maintainer 请帮忙看看这个问题
```

### 引用其他Issue
使用 `#Issue号码` 可以引用其他Issue：
```
这个问题可能和 #123 相关
```

## 👀 第五步：预览和检查

在提交前，务必预览你的内容！

### 操作步骤
1. **点击"Preview"标签页**
   - 在编辑框顶部，"Write"旁边有"Preview"
2. **仔细检查格式**
   - 标题是否清晰
   - 内容是否易读
   - 代码块是否正确显示
   - 图片是否正常加载
3. **检查内容完整性**
   - 是否包含了所有必要信息
   - 重现步骤是否清晰
   - 环境信息是否准确

### 常见格式问题
- **代码没有格式化**：确保使用了代码块语法
- **列表没有正确显示**：检查`-`或`1.`后面是否有空格
- **图片无法显示**：重新上传图片

## 🚀 第六步：提交Issue

确认无误后，就可以提交了！

### 操作步骤
1. **最后检查**
   - 标题是否准确
   - 内容是否完整
   - 格式是否正确

2. **点击"Submit new issue"按钮**
   - 这是一个绿色的按钮
   - 通常在编辑框的左下角

3. **提交成功后**
   - 页面会跳转到你刚创建的Issue页面
   - 你会看到Issue号码（如#124）
   - 系统会自动发送通知给项目维护者

### 侧边栏选项说明
**新手建议：除非项目文档明确要求，否则侧边栏选项都可以留空**

- **Assignees（指派人）**：留空，让维护者决定
- **Labels（标签）**：留空，维护者会添加合适的标签  
- **Projects（项目）**：留空
- **Milestone（里程碑）**：留空

## 📬 第七步：提交后的跟进

提交Issue只是开始，后续的互动同样重要。

### 关注通知
1. **邮件通知**
   - GitHub会发送邮件通知到你的注册邮箱
   - 包括新回复、状态变更等

2. **网站通知**
   - 点击GitHub右上角的通知图标（🔔）
   - 查看所有相关通知

### 回复互动
当维护者或其他用户回复时：

1. **及时回复**
   - 如果有人询问更多信息，尽快提供
   - 补充截图或详细描述

2. **保持礼貌**
   - 使用"请"、"谢谢"等礼貌用语
   - 即使对方态度不好，也要保持专业

3. **提供测试反馈**
   - 如果维护者提供了解决方案，及时测试并反馈结果

### 如何回复
在Issue页面底部有评论框：

```
┌─ Write ─ Preview ─────────────────────────┐
│                                           │
│  在这里输入回复内容                       │
│  同样支持Markdown语法                     │
│                                           │
└───────────────────────────────────────────┘
            [Comment] 按钮
```

### 关闭Issue
当问题解决后：

1. **由维护者关闭**：通常情况下，维护者会关闭Issue
2. **自己关闭**：如果问题自己解决了，可以点击"Close issue"按钮
3. **评论后关闭**：可以先添加解决方案的评论，再关闭

### Issue状态
- **Open（开放）**：问题还未解决
- **Closed（已关闭）**：问题已解决或不会处理

## ⚠️ 常见错误和注意事项

### 新手常犯的错误
1. **重复提交**：没有搜索就直接创建新Issue
2. **信息不足**：只说"有问题"不说具体是什么问题
3. **格式混乱**：不使用Markdown格式，代码直接贴在正文中
4. **环境信息缺失**：不提供操作系统、浏览器版本等关键信息
5. **标题过于宽泛**：使用"bug"、"问题"等无具体意义的标题

### 如何避免这些错误
- **仔细阅读项目的贡献指南**
- **使用我们提供的模板**
- **提交前预览内容**
- **多提供细节总比少了好**

## 🎉 恭喜你！

如果你完成了上述所有步骤，恭喜你已经成功提交了第一个GitHub Issue！

### 接下来可以做什么
1. **关注项目动态**：定期查看Issue的更新
2. **学习其他贡献方式**：比如提交代码、改进文档
3. **帮助其他新手**：在社区中分享你的经验
4. **继续改进**：根据反馈不断提高Issue质量

### 成长建议
- **多观察**：看看其他优质Issue是怎么写的
- **多练习**：在不同项目中尝试提交Issue
- **多学习**：了解更多开源贡献的知识

---

记住，每个开源贡献者都是从第一个Issue开始的。你的贡献，无论大小，都对开源社区有价值！

如果在操作过程中遇到任何问题，欢迎回到这个教程项目提交Issue，我们会帮助你解决。