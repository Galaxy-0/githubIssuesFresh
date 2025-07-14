# GitHub官方Issue模板指南

GitHub提供了官方的Issue模板功能，让项目维护者可以预设标准化的提交格式。作为贡献者，了解这些模板的使用方法非常重要。

## 📋 什么是GitHub Issue模板？

GitHub Issue模板是项目维护者预先设置的表单，用于：
- **标准化**：确保所有Issues包含必要信息
- **提高效率**：减少来回询问的沟通成本
- **分类管理**：不同类型的问题使用不同模板
- **质量保证**：引导贡献者提供完整信息

## 🎯 如何识别项目是否有Issue模板

### 方法1：查看Issues页面
当你点击"New issue"按钮时：

**有模板的项目：**
```
Choose a template
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

🐛 Bug report
Report a bug to help us improve
                                [Get started]

✨ Feature request  
Suggest an idea for this project
                                [Get started]

📖 Documentation issue
Report an issue with documentation
                                [Get started]

❓ Question
Ask a question about this project  
                                [Get started]

Don't see your issue here? Open a blank issue.
```

**没有模板的项目：**
直接进入Issue编辑页面，没有选择界面。

### 方法2：查看项目文件结构
项目根目录下是否有：
- `.github/ISSUE_TEMPLATE/` 目录
- `.github/issue_template.md` 文件
- `ISSUE_TEMPLATE.md` 文件

## 📝 如何使用Issue模板

### 第一步：选择合适的模板
根据你的问题类型选择：

| 模板类型 | 何时使用 | 常见图标 |
|---------|---------|---------|
| Bug report | 软件出现错误、异常行为 | 🐛 |
| Feature request | 希望添加新功能 | ✨ 💡 🚀 |
| Documentation | 文档错误、缺失、不清楚 | 📖 📚 📝 |
| Question | 使用问题、操作疑问 | ❓ 💬 🤔 |
| Performance | 性能问题、速度慢 | ⚡ 🚀 |
| Security | 安全漏洞、隐私问题 | 🔒 🛡️ |

### 第二步：按模板要求填写
模板通常包含：

1. **必填字段**（标记为Required）
2. **可选字段**（标记为Optional）
3. **预设选项**（下拉菜单、复选框）
4. **格式指导**（如何填写每个部分）

### 第三步：不要删除模板结构
⚠️ **重要提醒**：
- 不要删除模板中的标题和格式
- 即使某个部分不适用，也写"无"或"不适用"
- 保持模板的完整结构

## 🔧 常见的模板类型详解

### Bug报告模板
```markdown
**Bug描述**
简洁清楚地描述这个bug。

**重现步骤**
重现此行为的步骤：
1. 前往 '...'
2. 点击 '....'
3. 滚动到 '....'
4. 看到错误

**期望行为**
对你期望发生的情况的清晰简洁描述。

**截图**
如果适用，请添加截图以帮助解释你的问题。

**设备信息 (请完成以下信息):**
 - 操作系统: [如 iOS]
 - 浏览器 [如 chrome, safari]
 - 版本 [如 22]

**其他信息**
在此处添加有关问题的任何其他上下文。
```

### 功能请求模板
```markdown
**你的功能请求是否与问题相关？请描述。**
对你所遇到问题的清晰简洁描述。例如，当[...]时我总是感到沮丧

**描述你想要的解决方案**
对你想要的功能的清晰简洁描述。

**描述你考虑过的替代方案**
对你考虑过的任何替代解决方案或功能的清晰简洁描述。

**其他信息**
在此处添加有关功能请求的任何其他上下文或截图。
```

## 🎨 高级模板功能

### 表单字段类型
GitHub支持多种表单字段：

1. **文本输入框**
   ```yaml
   - type: input
     attributes:
       label: "Bug标题"
       placeholder: "简洁描述这个bug"
     validations:
       required: true
   ```

2. **多行文本框**
   ```yaml
   - type: textarea
     attributes:
       label: "详细描述"
       placeholder: "详细描述遇到的问题..."
   ```

3. **下拉选择**
   ```yaml
   - type: dropdown
     attributes:
       label: "操作系统"
       options:
         - Windows
         - macOS
         - Linux
   ```

4. **复选框**
   ```yaml
   - type: checkboxes
     attributes:
       label: "检查清单"
       options:
         - label: "我已搜索过现有issues"
           required: true
   ```

### 自动标签和指派
模板可以自动：
- 添加标签（如`bug`、`enhancement`）
- 指派给特定维护者
- 设置项目和里程碑

## ⚠️ 使用模板的注意事项

### 必须遵守的规则
1. **不要跳过必填字段**
2. **按照格式要求填写**
3. **提供真实准确的信息**
4. **保持礼貌的语言**

### 常见错误
❌ **错误做法**：
- 删除模板结构，自己随意写
- 在Bug模板中请求新功能
- 必填字段写"无"或留空
- 复制粘贴无关内容

✅ **正确做法**：
- 按照模板指引逐项填写
- 选择最符合问题性质的模板
- 提供所需的所有信息
- 使用清晰的表达

## 🛠️ 如果没有合适的模板怎么办？

### 选项1：使用最接近的模板
选择最相近的模板，在描述中说明差异：
```
注：此问题不完全符合Bug报告，但选择此模板因为...
```

### 选项2：使用空白Issue
大多数项目提供"Open a blank issue"选项：
- 点击模板选择页面底部的链接
- 自行按照项目贡献指南编写

### 选项3：联系维护者
如果经常遇到某类问题没有合适模板：
- 在讨论区提建议
- 联系项目维护者
- 建议添加新的模板类型

## 📊 模板使用的最佳实践

### 对于贡献者
1. **仔细阅读每个字段的说明**
2. **提供尽可能详细的信息**
3. **上传相关截图或文件**
4. **使用恰当的格式（代码块、列表等）**
5. **检查拼写和语法**

### 对于项目维护者
如果你是项目维护者，可以：
1. **创建清晰的模板**
2. **定期更新模板内容**
3. **添加使用指导**
4. **设置自动化标签**

## 🎯 实际案例分析

### 案例1：使用Bug报告模板
**场景**：网站登录功能在某个浏览器中无法正常工作

**正确使用模板**：
1. 选择"Bug report"模板
2. 在"Bug描述"中写明登录按钮无响应
3. 在"重现步骤"中详细列出操作流程
4. 在"期望行为"中说明应该跳转到首页
5. 在"设备信息"中提供浏览器版本
6. 上传截图显示问题界面

### 案例2：使用功能请求模板
**场景**：希望应用添加深色主题

**正确使用模板**：
1. 选择"Feature request"模板
2. 在问题描述中说明白天主题在夜间使用的不便
3. 在解决方案中描述深色主题的具体需求
4. 在替代方案中提及浏览器插件的局限性
5. 提供其他应用的深色主题截图参考

## 📚 相关资源

- [GitHub官方模板文档](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests)
- [模板语法参考](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/syntax-for-issue-forms)
- [最佳实践指南](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/configuring-issue-templates-for-your-repository)

---

记住，Issue模板是为了帮助你更好地表达问题，而不是增加负担。合理使用模板能让你的贡献更有效，也能获得更快的响应！