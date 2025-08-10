# 🌟 VSCode-Copilot-Chat-Viewer

**提取并可视化您在VS Code中隐藏的GitHub Copilot对话记录**

现代化的Discord风格聊天记录可视化工具，专为VS Code中的GitHub Copilot对话设计。

## 💡 为什么需要这个工具？

您是否曾经关闭VS Code后，发现找不到之前与Copilot的精彩对话了？别担心，您的聊天记录其实并没有被删除！

即使关闭了工作区，VS Code也会将所有Copilot聊天会话保存在计算机的特定位置。这个工具可以帮助您**提取、读取和可视化**那些隐藏的聊天记录，以美观、有序的格式展现。

### 🔍 重要发现

经过深入调查，我们发现VS Code将Copilot聊天记录存储在：
```
C:\Users\[用户名]\AppData\Roaming\Code\User\workspaceStorage\[工作区随机ID]\chatSessions\
```

这些JSON文件包含了您与Copilot的所有宝贵对话，但原始格式并不容易阅读。这就是我们工具的价值所在！

## ✨ 主要特性

- **Discord风格深色主题**: 专业的深色界面，灵感来源于Discord
- **多语言支持**: 一键切换中英文界面
- **智能解析**: 自动检测并解析GitHub Copilot JSON格式
- **响应式设计**: 完美适配桌面和移动设备
- **实时可视化**: 即时聊天记录渲染，流畅动画效果

## 🚀 快速开始

### 第一步：找到您的聊天记录
1. 打开文件资源管理器，导航到：
   ```
   C:\Users\[用户名]\AppData\Roaming\Code\User\workspaceStorage\
   ```
   **快捷方式**：按 `Win + R`，输入 `%APPDATA%\Code\User\workspaceStorage\` 然后按回车
   
2. 查找对应您VS Code工作区的文件夹

3. 在工作区目录中找到 `chatSessions` 文件夹

4. 从chatSessions文件夹中复制任何 `.json` 文件

### 第二步：可视化您的聊天记录
1. 在浏览器中打开 `chat-visualizer.html`
2. 点击语言切换按钮 (EN/中) 来切换界面语言
3. 上传您复制的JSON文件或使用 `demo-chat.json` 进行测试
4. 在美观的聊天界面中查看您的对话记录

### 💡 专业提示
- **多个工作区**：您可能有多个工作区文件夹 - 检查日期来找到最近的
- **文件大小**：较大的JSON文件通常包含更多聊天历史
- **备份建议**：考虑定期备份重要的聊天会话

## 📁 文件结构

```
Chat/
├── chat-visualizer.html           # 主要可视化工具
├── README.md                      # 英文说明文档
├── README-zh.md                   # 中文说明文档（本文件）
├── demo-chat.json                 # 演示聊天记录
├── test1.json                     # 示例聊天记录
└── refactor-handlers-chat.json    # 示例聊天记录
```

## 🌍 语言支持

- **中文界面**: 完整的中文用户界面和文档
- **English Interface**: 完整的英文界面和文档
- **一键切换**: 随时在两种语言间切换

## 📱 浏览器兼容性

- ✅ Chrome 60+
- ✅ Firefox 55+
- ✅ Safari 12+
- ✅ Edge 79+


## 📝 如何获取聊天记录

### 🔍 方法一：从VS Code存储位置提取（推荐）

1. **导航到VS Code存储位置**：
   ```
   C:\Users\[用户名]\AppData\Roaming\Code\User\workspaceStorage\
   ```
   
2. **查找您的工作区文件夹**：
   - 每个文件夹都有一个随机ID（例如：`a1b2c3d4e5f6...`）
   - 寻找与您最近项目匹配的文件夹
   - 检查创建/修改日期来确认

3. **定位聊天会话**：
   ```
   [工作区ID]\chatSessions\
   ```
   
4. **复制JSON文件**：
   - 文件以会话ID命名
   - 从此目录复制任何`.json`文件
   - 这些文件包含您的完整聊天历史

### 🎯 方法二：从GitHub Copilot导出

1. **直接导出**（如果可用）：
   - 在VS Code中使用GitHub Copilot扩展
   - 将聊天历史导出为JSON格式

### 🧪 方法三：使用演示文件

1. **先测试工具**：
   - 使用 `demo-chat.json` 测试功能
   - 这是一个包含示例对话的安全演示文件
   - 不包含任何个人信息或真实聊天数据

## 🔧 故障排除

### 查找聊天记录

**问：找不到workspaceStorage文件夹？**
答：
- 确保在文件资源管理器中显示隐藏文件（查看 → 隐藏的项目）
- 尝试快捷访问方法：`Win + R` → `%APPDATA%\Code\User\workspaceStorage\`
- AppData文件夹在Windows中默认是隐藏的

**问：找到了workspaceStorage但没有chatSessions文件夹？**
答：
- 不是所有工作区都有聊天会话
- 查找最近修改日期的文件夹
- 尝试检查其他工作区文件夹

**问：chatSessions文件夹是空的？**
答：
- 您可能在该工作区中没有与Copilot进行过对话
- 尝试检查其他工作区文件夹
- 确保您在VS Code中使用过GitHub Copilot聊天功能

### 常见问题

**问：文件无法解析？**
答：请确保文件是有效的JSON格式，且包含GitHub Copilot的聊天记录结构。

**问：界面显示异常？**
答：尝试刷新页面或使用推荐的浏览器（Chrome、Firefox、Edge）。

**问：语言切换不生效？**
答：清除浏览器缓存后重试，确保JavaScript已启用。

### 支持的文件格式

```json
{
  "version": 3,
  "requesterUsername": "用户名",
  "responderUsername": "GitHub Copilot",
  "requests": [
    {
      "requestId": "请求ID",
      "message": {
        "text": "用户消息内容"
      },
      "response": [
        {
          "value": "AI回复内容"
        }
      ]
    }
  ]
}
```

---

> 🚀 **准备好探索您的AI对话了吗？** 打开 `chat-visualizer.html` 开始可视化！

> 🌍 **International friendly**: Click the language toggle button to switch to English interface
