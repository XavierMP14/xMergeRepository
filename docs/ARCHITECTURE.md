# xMergeRepository Architecture

A comprehensive guide to understanding the architecture and structure of xMergeRepository.

## 🏗️ Overall Architecture

xMergeRepository is organized as a **monorepo** containing four distinct projects, each with its own technology stack and purpose.

```
xMergeRepository/
├── copilot-cli-skills/          # TypeScript/Node.js
├── mcp-dotnet-samples/          # C#/.NET 9
├── vscode-dotnettools/          # TypeScript/C#
├── copilot-spaces-skills/       # GitHub Skills
└── docs/                        # Shared documentation
```

---

## 📦 Project-Specific Architecture

### 1. Copilot CLI Skills

**Technology Stack:**
- TypeScript
- Node.js 20+
- GitHub Skills Framework

**Structure:**
```
copilot-cli-skills/
├── src/
│   ├── index.ts
│   ├── commands/
│   └── utils/
├── script/
│   ├── build-ui/
│   └── test
├── package.json
└── README.md
```

**Key Components:**
- CLI utilities for GitHub Copilot
- Issue management tools
- Application scaffolding

**Dependencies:**
- GitHub CLI API
- TypeScript compiler
- Jest for testing

---

### 2. MCP .NET Samples

**Technology Stack:**
- C# 12+
- .NET 9
- Model Context Protocol (MCP)

**Structure:**
```
mcp-dotnet-samples/
├── packages/
│   ├── McpSamples.Shared/       # Shared utilities
│   ├── AwesomeCopilot/          # MCP server samples
│   ├── MarkdownToHtml/          # HTML conversion
│   ├── TodoList/                # Todo management
│   └── OutlookEmail/            # Email integration
├── src/
│   ├── [Project].HybridApp/     # Entry point
│   └── [Project].Tests/         # Unit tests
├── .sln                         # Solution file
└── README.md
```

**Key Features:**
- **Hybrid Pattern:** Same code runs as STDIO or HTTP
- **Auto-Discovery:** Tools/Prompts auto-registered via attributes
- **Dependency Injection:** Built on ASP.NET Core DI container
- **Deployment:** Container-ready, Azure Functions support

**Architecture Layers:**
1. **Entry Point** - Program.cs (CLI/HTTP selection)
2. **Services** - Business logic and MCP handlers
3. **Shared Library** - Common utilities and extensions
4. **Data Access** - SQLite/EF Core (where applicable)

**Deployment Options:**
- Standalone console app
- Docker container (port 8080)
- Azure Functions
- Cloud Service

---

### 3. VSCode DotNet Tools

**Technology Stack:**
- TypeScript
- VS Code Extension API
- C# Development Kit

**Structure:**
```
vscode-dotnettools/
├── src/
│   ├── extension.ts
│   ├── commands/
│   ├── providers/
│   └── utils/
├── test/
├── .vscode/
│   └── launch.json
├── package.json
└── README.md
```

**Key Components:**
- VS Code extension API integration
- C# language support enhancement
- Development tools integration

**Extension Points:**
- Commands
- Language features
- Debugging support
- Test framework integration

---

### 4. Copilot Spaces Skills

**Technology Stack:**
- GitHub Skills Framework
- Markdown
- GitHub Actions

**Structure:**
```
copilot-spaces-skills/
├── .github/
│   ├── workflows/
│   └── ISSUE_TEMPLATE/
├── docs/
│   └── lessons/
├── exercises/
│   └── [exercise-name]/
└── README.md
```

**Key Features:**
- Interactive learning modules
- Automated feedback via GitHub Actions
- Progressive difficulty levels
- Real-world scenarios

---

## 🔄 Monorepo Workflow

### Shared Configuration
- **Root .gitignore** - Common exclusions
- **Root package.json** - Workspace management (if applicable)
- **.github/workflows/** - CI/CD for all projects
- **docs/** - Shared documentation

### Build & Test Orchestration
```bash
# Test all projects
npm test                    # TypeScript projects
dotnet test                 # .NET projects

# Build all projects
npm run build               # TypeScript projects
dotnet build                # .NET projects
```

### Dependency Management
- Each project manages its own dependencies
- Shared utilities in `mcp-dotnet-samples/packages/McpSamples.Shared/`
- No cross-project tight coupling

---

## 🔗 Inter-Project Dependencies

### Direct Dependencies
- **VSCode DotNet Tools** ← Uses C# Dev Kit APIs
- **MCP .NET Samples** ← Standalone, no internal deps
- **Copilot CLI Skills** ← Uses GitHub API
- **Copilot Spaces Skills** ← Uses GitHub Skills framework

### Shared Resources
- Documentation (docs/)
- GitHub workflows (.github/workflows/)
- Issue templates (.github/ISSUE_TEMPLATE/)
- Contribution guidelines

---

## 🚀 Deployment Architecture

### Development Environment
```
Developer Machine
├── xMergeRepository (cloned)
│   ├── copilot-cli-skills
│   │   └── npm install && npm run dev
│   ├── mcp-dotnet-samples
│   │   └── dotnet run
│   ├── vscode-dotnettools
│   │   └── code --extensionDevelopmentPath=.
│   └── copilot-spaces-skills
│       └── GitHub Actions runner
```

### Production Deployment

**Copilot CLI Skills:**
- npm package (if published)
- GitHub Actions integration

**MCP .NET Samples:**
- Docker containers
- Azure Functions
- Container Registry (ghcr.io)

**VSCode DotNet Tools:**
- VS Code Marketplace
- Auto-update via VS Code

**Copilot Spaces Skills:**
- GitHub repository
- GitHub Actions
- Student environments

---

## 🔐 Security Architecture

### Authentication & Authorization
- GitHub token management (GitHub Actions secrets)
- Azure credentials (for deployments)
- VS Code extension sandbox

### Data Protection
- No hardcoded secrets
- Environment variables for sensitive data
- Secure token handling in CI/CD

### Code Security
- Dependency scanning
- Static code analysis
- Regular security audits

---

## 📊 Testing Architecture

### Unit Tests
- TypeScript: Jest
- .NET: xUnit/NUnit
- Isolated component testing

### Integration Tests
- End-to-end scenarios
- API contract testing
- Database integration (for applicable projects)

### E2E Tests (where applicable)
- Full workflow testing
- User scenario validation
- Environment-based testing

---

## 📈 Performance Considerations

### Optimization Areas
1. **Copilot CLI Skills**
   - Command response time
   - Memory footprint

2. **MCP .NET Samples**
   - HTTP request latency
   - Container startup time
   - Database query optimization

3. **VSCode DotNet Tools**
   - Extension activation time
   - Language service responsiveness

---

## 🎯 Design Principles

1. **Separation of Concerns**
   - Each project has clear boundaries
   - Loose coupling between projects

2. **Reusability**
   - Shared code in dedicated libraries
   - Common patterns documented

3. **Scalability**
   - Container-ready architecture
   - Horizontal scaling support

4. **Maintainability**
   - Clear documentation
   - Consistent code standards
   - Automated testing

5. **Developer Experience**
   - Clear setup instructions
   - Fast feedback loop
   - Comprehensive examples

---

## 🔄 CI/CD Pipeline

### GitHub Actions Workflows
- **Build:** Compile all projects
- **Test:** Run test suites
- **Lint:** Code quality checks
- **Security:** Dependency scanning
- **Deploy:** Container publishing (applicable projects)

### Branch Protection
- All tests must pass
- Code review required
- Linting checks required

---

## 📚 Additional Resources

- [Getting Started](./GETTING_STARTED.md)
- [Contributing Guidelines](./CONTRIBUTING.md)
- Project-specific READMEs in each directory

---

**Last Updated:** June 3, 2026
