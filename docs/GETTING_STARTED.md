# Getting Started with xMergeRepository

Welcome to **xMergeRepository**! This guide will help you get up and running quickly.

## 📋 Prerequisites

Before you begin, ensure you have the following installed:

### For All Projects
- **Git** (2.30+)
- **GitHub account** with access to the repository

### For Copilot CLI Skills & VSCode DotNet Tools
- **Node.js** (20.0+)
- **npm** (10.0+)

### For MCP .NET Samples
- **.NET SDK** (9.0+)
- **dotnet CLI**

### For VSCode DotNet Tools Development
- **Visual Studio Code** (latest)
- **C# Dev Kit** extension

### For Copilot Spaces Skills
- **GitHub Actions** (already enabled in repository)

---

## 🚀 Quick Start

### 1. Clone the Repository

```bash
git clone https://github.com/XavierMP14/xMergeRepository.git
cd xMergeRepository
```

### 2. Choose Your Project

Navigate to the project folder:

```bash
# TypeScript/Node.js projects
cd copilot-cli-skills
# or
cd vscode-dotnettools

# .NET projects
cd mcp-dotnet-samples

# GitHub Skills exercises
cd copilot-spaces-skills
```

---

## 🎯 Project-Specific Setup

### A. Copilot CLI Skills

**Install dependencies:**
```bash
cd copilot-cli-skills
npm install
```

**Run the application:**
```bash
npm run dev
```

**Run tests:**
```bash
npm test
```

**Build for production:**
```bash
npm run build
```

**Available scripts:**
```bash
npm run dev          # Development server
npm run build        # Production build
npm run test         # Run tests
npm run lint         # Lint code
npm run format       # Format code
```

---

### B. MCP .NET Samples

**Restore dependencies:**
```bash
cd mcp-dotnet-samples
dotnet restore
```

**Build the project:**
```bash
dotnet build
```

**Run tests:**
```bash
dotnet test
```

**Run a specific sample (STDIO mode):**
```bash
dotnet run --project ./markdown-to-html/src/McpSamples.MarkdownToHtml.HybridApp
```

**Run a specific sample (HTTP mode):**
```bash
dotnet run --project ./todo-list/src/McpSamples.TodoList.HybridApp -- --http
```

**Available samples:**
- **awesome-copilot** - Metadata and instruction management
- **markdown-to-html** - Convert markdown to HTML
- **todo-list** - In-memory todo management with SQLite
- **outlook-email** - Email integration sample

**Docker deployment:**
```bash
docker build -f Dockerfile.todo-list -t todo-list:latest .
docker run -i --rm -p 8080:8080 todo-list:latest
```

---

### C. VSCode DotNet Tools

**Install dependencies:**
```bash
cd vscode-dotnettools
npm install
```

**Development mode (launch in VSCode):**
```bash
# Open VSCode
code .

# Press F5 to launch the extension in debug mode
```

**Run tests:**
```bash
npm test
```

**Build extension:**
```bash
npm run build
```

**Package extension (for distribution):**
```bash
npm run package
```

---

### D. Copilot Spaces Skills

**No installation required!** This is a GitHub Skills exercise.

1. Visit the repository: [xMergeRepository/copilot-spaces-skills](./copilot-spaces-skills)
2. Open an issue to start the exercise
3. Follow the instructions provided by the GitHub bot
4. Complete the interactive challenges

---

## 📚 Common Commands

### TypeScript/JavaScript Projects

```bash
# Installation
npm install

# Development
npm run dev

# Build
npm run build

# Testing
npm test

# Linting
npm run lint

# Formatting
npm run format
```

### .NET Projects

```bash
# Restore dependencies
dotnet restore

# Build
dotnet build

# Test
dotnet test

# Run
dotnet run

# Clean
dotnet clean
```

---

## 🧪 Running Tests

### Copilot CLI Skills
```bash
cd copilot-cli-skills
npm test
```

### MCP .NET Samples
```bash
cd mcp-dotnet-samples
dotnet test
```

### VSCode DotNet Tools
```bash
cd vscode-dotnettools
npm test
```

---

## 📖 Project Documentation

Each project has its own README with detailed information:

- [copilot-cli-skills/README.md](../copilot-cli-skills/README.md)
- [mcp-dotnet-samples/README.md](../mcp-dotnet-samples/README.md)
- [vscode-dotnettools/README.md](../vscode-dotnettools/README.md)
- [copilot-spaces-skills/README.md](../copilot-spaces-skills/README.md)

---

## 🔧 Troubleshooting

### Node.js / npm Issues

**Problem:** `npm: command not found`
```bash
# Install Node.js from https://nodejs.org
# Verify installation
node --version
npm --version
```

**Problem:** Permission denied during npm install
```bash
# Clear npm cache and retry
npm cache clean --force
npm install
```

### .NET Issues

**Problem:** `.NET SDK not found`
```bash
# Install .NET from https://dotnet.microsoft.com/download
# Verify installation
dotnet --version
```

**Problem:** Build fails
```bash
# Clean and rebuild
dotnet clean
dotnet restore
dotnet build
```

### Git Issues

**Problem:** `fatal: not a git repository`
```bash
# Ensure you're in the repository directory
cd xMergeRepository
git status
```

**Problem:** `Authentication failed`
```bash
# Generate a new GitHub token
# https://github.com/settings/tokens
# Use: git clone https://YOUR_TOKEN@github.com/XavierMP14/xMergeRepository.git
```

---

## 🤝 Contributing

Ready to contribute? Check out our [Contributing Guidelines](./CONTRIBUTING.md) for:
- How to fork and create feature branches
- Code standards for each project
- Pull request process
- Commit message conventions

---

## 📝 Environment Setup (Optional)

### VS Code Extensions (Recommended)

```json
{
  "recommendations": [
    "ms-vscode.cpptools",
    "ms-dotnettools.csharp",
    "ms-dotnettools.vscode-dotnet-runtime",
    "esbenp.prettier-vscode",
    "dbaeumer.vscode-eslint"
  ]
}
```

### Git Configuration (Recommended)

```bash
# Configure git for this repository
git config user.name "Your Name"
git config user.email "your.email@example.com"

# Enable automatic line ending conversion
git config core.autocrlf true
```

---

## 🚀 Next Steps

1. **Pick a project** that interests you
2. **Read the project README** for detailed information
3. **Set up your development environment** using the steps above
4. **Explore the code** and get familiar with the structure
5. **Start contributing** (see Contributing Guidelines)
6. **Ask questions** in GitHub Issues if you need help

---

## 📞 Support & Resources

- **Documentation:** [docs/](../)
- **Architecture:** [docs/ARCHITECTURE.md](./ARCHITECTURE.md)
- **Contributing:** [docs/CONTRIBUTING.md](./CONTRIBUTING.md)
- **Issues:** [GitHub Issues](https://github.com/XavierMP14/xMergeRepository/issues)
- **Discussions:** [GitHub Discussions](https://github.com/XavierMP14/xMergeRepository/discussions)

---

## 🎓 Learning Resources

### TypeScript/JavaScript
- [Node.js Official Documentation](https://nodejs.org/docs/)
- [TypeScript Handbook](https://www.typescriptlang.org/docs/)
- [Jest Testing Framework](https://jestjs.io/)

### .NET/C#
- [.NET Documentation](https://learn.microsoft.com/en-us/dotnet/)
- [C# Programming Guide](https://learn.microsoft.com/en-us/dotnet/csharp/)
- [ASP.NET Core](https://learn.microsoft.com/en-us/aspnet/core/)

### GitHub
- [GitHub Docs](https://docs.github.com)
- [GitHub Skills](https://skills.github.com)
- [GitHub API Documentation](https://docs.github.com/en/rest)

---

## ✨ Happy Coding!

You're all set! Start exploring the projects and happy coding. 🚀

If you encounter any issues, check the troubleshooting section or open an issue on GitHub.

**Last Updated:** June 3, 2026
