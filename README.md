# xMergeRepository 🚀

A unified repository consolidating all XavierMP14 projects into a single, organized monorepo structure.

## 📚 Project Overview

**xMergeRepository** brings together multiple technology initiatives under one roof:

| Project | Directory | Technology | Status |
|---------|-----------|-----------|--------|
| **Copilot CLI Skills** | `copilot-cli-skills/` | TypeScript/Node.js | Active |
| **MCP .NET Samples** | `mcp-dotnet-samples/` | C#/.NET 9 | Active |
| **VSCode DotNet Tools** | `vscode-dotnettools/` | TypeScript/C# | Active |
| **Copilot Spaces Skills** | `copilot-spaces-skills/` | GitHub Skills | Active |

---

## 📁 Repository Structure

```
xMergeRepository/
├── copilot-cli-skills/
│   ├── README.md
│   ├── package.json
│   ├── src/
│   └── script/
│
├── mcp-dotnet-samples/
│   ├── README.md
│   ├── packages/
│   ├── src/
│   └── docs/
│
├── vscode-dotnettools/
│   ├── README.md
│   ├── src/
│   └── docs/
│
├── copilot-spaces-skills/
│   ├── README.md
│   └── exercises/
│
├── .github/
│   ├── workflows/
│   ├── ISSUE_TEMPLATE/
│   └── copilot-instructions.md
│
├── docs/
│   ├── GETTING_STARTED.md
│   ├── ARCHITECTURE.md
│   └── CONTRIBUTING.md
│
└── README.md (this file)
```

---

## 🚀 Getting Started

### Prerequisites
- **Node.js 20+** (for Copilot CLI Skills)
- **.NET 9+** (for MCP .NET Samples)
- **Git** (for repository management)

### Installation

```bash
# Clone the repository
git clone https://github.com/XavierMP14/xMergeRepository.git
cd xMergeRepository

# Install dependencies (per project)
cd copilot-cli-skills
npm install

cd ../mcp-dotnet-samples
dotnet restore

cd ../vscode-dotnettools
npm install
```

---

## 📖 Projects Summary

### 1. Copilot CLI Skills
**Location:** `copilot-cli-skills/`

Learn how to use GitHub Copilot CLI for issue management and building applications.
- Create applications with the Copilot CLI
- GitHub Skills exercise framework
- Interactive hands-on learning

**Start here:** `copilot-cli-skills/README.md`

---

### 2. MCP .NET Samples
**Location:** `mcp-dotnet-samples/`

Comprehensive samples for creating and using MCP (Model Context Protocol) servers and clients with .NET.

Features:
- Hybrid MCP servers (STDIO + HTTP)
- Multiple sample applications (awesome-copilot, markdown-to-html, todo-list, outlook-email)
- Shared library (`McpSamples.Shared`)
- Azure Functions deployment support
- OpenAPI documentation

**Start here:** `mcp-dotnet-samples/README.md`

---

### 3. VSCode DotNet Tools
**Location:** `vscode-dotnettools/`

Feedback repository for the C# Dev Kit and related extensions from Visual Studio Code.
- Issue tracking and feedback
- Feature requests
- Bug reports for C# development tools

**Start here:** `vscode-dotnettools/README.md`

---

### 4. Copilot Spaces Skills
**Location:** `copilot-spaces-skills/`

GitHub Skills exercise for scaling institutional knowledge using Copilot Spaces.
- Learn about Copilot Spaces
- Scale knowledge management
- Interactive exercises

**Start here:** `copilot-spaces-skills/README.md`

---

## 🤝 Contributing

We welcome contributions! Please see our [Contributing Guidelines](./docs/CONTRIBUTING.md) for details.

### Development Workflow

1. Create a feature branch: `git checkout -b feature/your-feature`
2. Make your changes
3. Run tests and lint checks
4. Commit with clear messages: `git commit -m "feat: add your feature"`
5. Push to your fork and create a Pull Request

### Code Standards

- **TypeScript/JavaScript:** Follow ESLint config
- **.NET/C#:** Follow StyleCop analyzers
- **Commits:** Follow Conventional Commits
- **Documentation:** Keep README.md files updated

---

## 📋 Project-Specific Commands

### Copilot CLI Skills
```bash
cd copilot-cli-skills
npm install
npm run build
npm test
```

### MCP .NET Samples
```bash
cd mcp-dotnet-samples
dotnet build
dotnet test
dotnet run --project ./[sample]/src/[Sample].HybridApp
```

### VSCode DotNet Tools
```bash
cd vscode-dotnettools
npm install
npm run build
```

---

## 🔗 Related Resources

- [GitHub MCP Server](https://github.com/github/github-mcp-server)
- [Azure DevOps MCP](https://github.com/microsoft/azure-devops-mcp)
- [VS Code Documentation](https://code.visualstudio.com/docs)
- [Web Platform Features](https://github.com/web-platform-dx/web-features)

---

## 📝 Documentation

- [Getting Started](./docs/GETTING_STARTED.md)
- [Architecture Overview](./docs/ARCHITECTURE.md)
- [Contributing Guide](./docs/CONTRIBUTING.md)
- [Project-Specific READMEs](#-projects-summary)

---

## 🎯 Current Status

| Component | Status | Last Updated |
|-----------|--------|--------------|
| Copilot CLI Skills | ✅ Active | 2026-06-03 |
| MCP .NET Samples | ✅ Active | 2026-06-03 |
| VSCode DotNet Tools | ✅ Active | 2026-06-03 |
| Copilot Spaces Skills | ✅ Active | 2026-06-03 |

---

## 🐛 Issues & Support

Found a bug? Have a feature request? Please open an issue on GitHub:
- [Report a Bug](https://github.com/XavierMP14/xMergeRepository/issues/new?labels=bug)
- [Request a Feature](https://github.com/XavierMP14/xMergeRepository/issues/new?labels=enhancement)

---

## 📄 License

This repository contains multiple projects with potentially different licenses. Please check individual project directories for their specific license information.

---

## 🌟 Acknowledgments

Built with passion by **@XavierMP14** and contributors.

Special thanks to:
- GitHub for the Skills framework
- Microsoft for .NET and VS Code
- The MCP (Model Context Protocol) community
- All contributors and maintainers

---

## 📞 Contact & Social

- GitHub: [@XavierMP14](https://github.com/XavierMP14)
- Issues: [GitHub Issues](https://github.com/XavierMP14/xMergeRepository/issues)

---

**Last Updated:** June 3, 2026
**Version:** 1.0.0

✨ *"Merging excellence, one repository at a time."* ✨
