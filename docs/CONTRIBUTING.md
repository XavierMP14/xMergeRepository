# Contributing to xMergeRepository

Thank you for your interest in contributing! We welcome contributions from everyone.

## 🚀 Getting Started

### 1. Fork and Clone
```bash
git clone https://github.com/XavierMP14/xMergeRepository.git
cd xMergeRepository
```

### 2. Create a Feature Branch
```bash
git checkout -b feature/your-feature-name
```

### 3. Make Your Changes
- Keep changes focused and atomic
- Follow the code standards for your project
- Update documentation as needed

### 4. Commit with Clear Messages
We follow [Conventional Commits](https://www.conventionalcommits.org/):

```bash
git commit -m "feat: add new feature"
git commit -m "fix: resolve bug in component"
git commit -m "docs: update README"
git commit -m "refactor: improve code structure"
```

### 5. Push and Create a Pull Request
```bash
git push origin feature/your-feature-name
```

Then open a PR on GitHub with a clear description of your changes.

---

## 📋 Code Standards

### TypeScript/JavaScript (Copilot CLI Skills, VSCode DotNet Tools)
- Use ESLint for linting
- Use Prettier for formatting
- Follow camelCase for variables and functions
- Use PascalCase for classes and components

```bash
npm run lint
npm run format
```

### .NET/C# (MCP .NET Samples)
- Follow StyleCop analyzers
- Use PascalCase for public members
- Document public APIs with XML comments
- Target .NET 9+

```bash
dotnet build
dotnet test
```

### Commits
- Use present tense: "add feature" not "added feature"
- Use imperative mood: "move cursor to..." not "moves cursor to..."
- Reference issues when applicable: "fixes #123"

---

## 🧪 Testing

Before submitting a PR, ensure all tests pass:

### Copilot CLI Skills & VSCode DotNet Tools
```bash
npm test
```

### MCP .NET Samples
```bash
dotnet test
```

### All Projects
```bash
# Run linting
npm run lint  # or dotnet build

# Run tests
npm test      # or dotnet test
```

---

## 📝 Documentation

When contributing, please update:
- **README.md** - If adding new features
- **docs/** - For architectural changes
- **Code comments** - For complex logic
- **API documentation** - For public APIs

---

## 🔍 Pull Request Process

1. **Create a descriptive PR title**
   - ✅ Good: "feat: add authentication to MCP server"
   - ❌ Bad: "Update code"

2. **Write a clear PR description**
   - What problem does this solve?
   - How does it solve it?
   - Any breaking changes?

3. **Link related issues**
   - Use `closes #123` to auto-close issues

4. **Ensure CI passes**
   - All tests must pass
   - Linting must pass
   - No conflicts with main branch

5. **Request review**
   - At least one approval required
   - Address feedback promptly

---

## 📊 Project Guidelines

### Copilot CLI Skills
- TypeScript with latest Node.js features
- Follow the existing folder structure
- Include unit tests for new features
- Update exercise documentation

### MCP .NET Samples
- .NET 9+ target framework
- Follow the hybrid pattern (STDIO + HTTP)
- Include sample configurations
- Document deployment scenarios
- Auto-discovery of tools/prompts

### VSCode DotNet Tools
- Report bugs and feedback clearly
- Include reproduction steps
- Attach error logs if applicable
- Test in VSCode insiders build

### Copilot Spaces Skills
- Follow GitHub Skills exercise format
- Include clear learning objectives
- Provide hands-on activities
- Test exercise flow end-to-end

---

## 🐛 Reporting Bugs

Use the bug report template:

```markdown
## Description
Clear and concise description of the bug.

## Steps to Reproduce
1. Step one
2. Step two
3. Step three

## Expected Behavior
What should happen?

## Actual Behavior
What actually happens?

## Environment
- OS: [e.g., Windows 11, macOS 14]
- Runtime: [e.g., Node.js 20.10, .NET 9.0]
- Project: [e.g., mcp-dotnet-samples]

## Logs/Screenshots
Attach relevant logs or screenshots.
```

---

## 💡 Feature Requests

Use the feature request template:

```markdown
## Description
What feature would you like to see?

## Use Case
Why do you need this feature?

## Proposed Solution
How would you implement this?

## Alternatives
Any alternative approaches?
```

---

## 🤝 Code Review Process

- Be respectful and constructive
- Ask clarifying questions
- Suggest improvements
- Acknowledge good work
- Aim for consensus, not perfection

---

## 📚 Resources

- [Conventional Commits](https://www.conventionalcommits.org/)
- [GitHub Flow Guide](https://guides.github.com/introduction/flow/)
- [Node.js Best Practices](https://nodejs.org/en/docs/guides/)
- [.NET Coding Conventions](https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/coding-style/coding-conventions)

---

## ❓ Questions?

- Open a discussion on GitHub
- Check existing issues for similar questions
- Create a new issue with your question

---

## 🎉 Code of Conduct

Please note that this project is released with a [Code of Conduct](./CODE_OF_CONDUCT.md). By participating in this project you agree to abide by its terms.

---

Thank you for contributing! Your efforts help make xMergeRepository better for everyone. 🙌
