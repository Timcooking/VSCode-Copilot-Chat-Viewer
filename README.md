# 🌟 VSCode-Copilot-Chat-Viewer

**Extract and visualize your hidden GitHub Copilot chat history from VS Code**

[![Live Demo](https://img.shields.io/badge/🚀_Live_Demo-Try_Now-blue?style=for-the-badge)](https://timcooking.github.io/VSCode-Copilot-Chat-Viewer/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](https://opensource.org/licenses/MIT)

## 💡 Why This Tool?

When you close VS Code, your Copilot chat history seems to disappear - but it's actually stored locally! This tool helps you **recover and visualize** those conversations in a beautiful Discord-style interface.

## 🎯 Key Features

- 🎨 **Discord-style dark theme** - Modern, professional interface
- 🌍 **Multi-language support** - Switch between English/Chinese
- 📱 **Responsive design** - Works on desktop and mobile
- 🔒 **Privacy-first** - All processing happens locally
- ⚡ **Zero dependencies** - Pure HTML/CSS/JavaScript

## 🚀 Quick Start

### 1. Find Your Chat Files
Navigate to: `C:\Users\[YourUsername]\AppData\Roaming\Code\User\workspaceStorage\`

**Quick tip**: Press `Win + R`, type `%APPDATA%\Code\User\workspaceStorage\` and hit Enter

### 2. Extract Chat Records
- Look for folders with random IDs (your workspaces)
- Find the `chatSessions` folder
- Copy any `.json` file from there

### 3. Visualize
- Open the [**Live Demo**](https://timcooking.github.io/VSCode-Copilot-Chat-Viewer/)
- Upload your JSON file
- Enjoy your conversation history!

## 📝 Testing

Don't have chat files yet? Use our [`demo-chat.json`](demo-chat.json) to test the tool.

## 🛠️ Local Usage

1. Download this repository
2. Open `index.html` in your browser
3. Upload your chat files

## 📱 Browser Support

Chrome, Firefox, Safari, Edge (modern versions)

## 🔧 Troubleshooting

**Can't find files?** Make sure hidden files are visible in Windows Explorer.

**File won't parse?** Ensure it's a valid JSON from VS Code's chatSessions folder.

## 🤝 Contributing

Issues and pull requests welcome! See [LICENSE](LICENSE) for details.

---

> 💬 **Rediscover your AI conversations** - Never lose your valuable Copilot chats again!

> 🌍 **中文文档**: 查看 [README-zh.md](README-zh.md) 获取中文说明

**Extract and Visualize Your H## 📁 File Structure

```
VSCode-Copilot-Chat-Viewer/
├── index.html                     # Main application (GitHub Pages entry)
├── chat-visualizer.html           # Alternative entry point
├── README.md                      # English documentation
├── README-zh.md                   # Chinese documentation
├── demo-chat.json                 # Demo chat record for testing
├── test1.json                     # Sample chat record
├── refactor-handlers-chat.json    # Sample chat record
├── LICENSE                        # MIT License
├── _config.yml                    # Jekyll configuration
├── .gitignore                     # Git ignore rules
└── .github/
    └── workflows/
        └── pages.yml              # GitHub Actions for auto-deployment
```b Copilot Conversations in VS Code**

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Live%20Demo-blue?style=flat-square&logo=github)](https://timcooking.github.io/VSCode-Copilot-Chat-Viewer/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](https://opensource.org/licenses/MIT)
[![GitHub stars](https://img.shields.io/github/stars/Timcooking/VSCode-Copilot-Chat-Viewer?style=flat-square)](https://github.com/Timcooking/VSCode-Copilot-Chat-Viewer/stargazers)

A modern, Discord-style chat record visualizer for GitHub Copilot in VS Code conversations.

## 🚀 Live Demo

**[Try it now on GitHub Pages!](https://timcooking.github.io/VSCode-Copilot-Chat-Viewer/)**

No installation required - just open the link and start visualizing your chat records!

## 💡 Why This Tool?

Have you ever closed VS Code and then realized you can't find your previous Copilot chat conversations? Don't worry - your chat records aren't actually deleted! 

Even after closing your workspace, VS Code stores all your Copilot chat sessions in a specific location on your computer. This tool helps you **extract, read, and visualize** those hidden chat records in a beautiful, organized format.

### 🔍 The Discovery

After some investigation, we found that VS Code stores Copilot chat records in:
```
C:\Users\[YourUsername]\AppData\Roaming\Code\User\workspaceStorage\[RandomWorkspaceID]\chatSessions\
```

These JSON files contain all your valuable conversations with Copilot, but they're not easily readable in their raw format. That's where our tool comes in!

## ✨ Features

- **Discord-style Dark Theme**: Professional dark interface inspired by Discord
- **Multi-language Support**: Switch between Chinese and English with one click
- **Smart Parsing**: Automatically detects and parses GitHub Copilot JSON format
- **Responsive Design**: Works perfectly on desktop and mobile devices
- **Real-time Visualization**: Instant chat record rendering with smooth animations

## 🚀 Quick Start

### Step 1: Find Your Chat Records
1. Open File Explorer and navigate to:
   ```
   C:\Users\[YourUsername]\AppData\Roaming\Code\User\workspaceStorage\
   ```
   **Quick tip**: Press `Win + R`, type `%APPDATA%\Code\User\workspaceStorage\` and press Enter
   
2. Look for folders corresponding to your VS Code workspaces

3. Find the `chatSessions` folder within your workspace directory

4. Copy any `.json` file from the chatSessions folder

### Step 2: Visualize Your Chats
1. Open `chat-visualizer.html` in your browser
2. Click the language toggle button (EN/中) to switch languages
3. Upload your copied JSON file or use `demo-chat.json` for testing
4. View your conversations in a beautiful chat interface

### 💡 Pro Tips
- **Multiple workspaces**: You may have multiple workspace folders - check dates to find recent ones
- **File sizes**: Larger JSON files usually contain more chat history
- **Backup**: Consider backing up important chat sessions regularly

## 📁 File Structure

```
Chat/
├── chat-visualizer.html           # Main visualization tool
├── README.md                      # This file (English)
├── README-zh.md                   # Chinese documentation
├── demo-chat.json                 # Demo chat record for testing
├── test1.json                     # Sample chat record
└── refactor-handlers-chat.json    # Sample chat record
```

## 🌍 Language Support

- **中文界面**: 完整的中文用户界面和文档
- **English Interface**: Full English UI and documentation
- **One-click Switch**: Toggle between languages anytime

## 📱 Browser Compatibility

- ✅ Chrome 60+
- ✅ Firefox 55+
- ✅ Safari 12+
- ✅ Edge 79+

## 🎯 Use Cases

- **Learning Review**: Revisit your AI-assisted learning journey
- **Project Documentation**: Visualize development conversations
- **Team Sharing**: Share interesting AI interactions
- **Presentation**: Showcase AI collaboration in meetings

## 🛠️ Technical Details

- **Zero Dependencies**: Pure HTML/CSS/JavaScript
- **Offline Ready**: Works without internet connection
- **Lightweight**: Fast loading and smooth performance
- **Privacy First**: All processing done locally in browser

## 📝 How to Get Chat Records

### 🔍 Method 1: Extract from VS Code Storage (Recommended)

1. **Navigate to VS Code storage location**:
   ```
   C:\Users\[YourUsername]\AppData\Roaming\Code\User\workspaceStorage\
   ```
   
2. **Find your workspace folder**:
   - Each folder has a random ID (e.g., `a1b2c3d4e5f6...`)
   - Look for folders that match your recent projects
   - Check the creation/modification dates

3. **Locate chat sessions**:
   ```
   [WorkspaceID]\chatSessions\
   ```
   
4. **Copy the JSON files**:
   - Files are named with session IDs
   - Copy any `.json` file from this directory
   - These contain your complete chat history

### 🎯 Method 2: Export from GitHub Copilot

1. **Direct export** (if available):
   - Use GitHub Copilot extension in VS Code
   - Export chat history as JSON format

### 🧪 Method 3: Use Demo Files

1. **Test the tool first**:
   - Use `demo-chat.json` for testing functionality
   - This is a safe demo file with sample conversations
   - Contains no personal information or real chat data

## 🔧 Troubleshooting

### Finding Chat Records

**Q: Can't find the workspaceStorage folder?**
A: 
- Make sure to show hidden files in File Explorer (View → Hidden items)
- Try the quick access method: `Win + R` → `%APPDATA%\Code\User\workspaceStorage\`
- The AppData folder is hidden by default in Windows

**Q: Found workspaceStorage but no chatSessions folder?**
A: 
- Not all workspaces have chat sessions
- Look for folders with recent modification dates
- Try opening a different workspace folder

**Q: Empty chatSessions folder?**
A: 
- You may not have had any Copilot conversations in that workspace
- Try checking other workspace folders
- Ensure you've used GitHub Copilot chat feature in VS Code

### Common Issues

**Q: File cannot be parsed?**
A: Make sure the file is valid JSON format and contains GitHub Copilot chat record structure.

**Q: Interface display issues?**
A: Try refreshing the page or use recommended browsers (Chrome, Firefox, Edge).

**Q: Language toggle not working?**
A: Clear browser cache and retry, ensure JavaScript is enabled.

### Supported File Format

```json
{
  "version": 3,
  "requesterUsername": "Username",
  "responderUsername": "GitHub Copilot",
  "requests": [
    {
      "requestId": "request_id",
      "message": {
        "text": "User message content"
      },
      "response": [
        {
          "value": "AI response content"
        }
      ]
    }
  ]
}
```

---

> 🚀 **Ready to explore your AI conversations?** Open `chat-visualizer.html` and start visualizing!

> 🌍 **国际友好**: 点击右上角的语言切换按钮可切换到中文界面
