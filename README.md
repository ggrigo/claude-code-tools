# Claude Code Tools

A collection of tools and configurations that enhance Claude Code's capabilities for development workflows.

## 🎯 Start Here: CLAUDE.md (No Installation Required!)

**Before installing any tools**, create a `CLAUDE.md` file in your project root. This is the single most impactful enhancement with zero configuration required.

### Quick Start
1. Create `CLAUDE.md` in your project root
2. Copy our [template](templates/CLAUDE.md.template) and customize it
3. That's it! Claude Code automatically loads it every session

**Why start with CLAUDE.md?**
- Zero installation or configuration
- Works 100% of the time for everyone  
- Immediate productivity boost
- Foundation for all other enhancements

📖 **[Full CLAUDE.md Guide](docs/CLAUDE_MD_GUIDE.md)** - Complete documentation and best practices

---

## Purpose

This repository provides:
1. Documentation of tools and configurations for Claude Code
2. Installation instructions for Claude Code to replicate setups
3. Templates and guides for maximum productivity

## How to Use This Repository

Simply ask Claude Code to:
1. Read this README for an overview
2. Start with CLAUDE.md (no installation needed!)
3. Then install additional tools as needed

## Tools & Configurations

### 1. Configuration Files (No Installation Required)

| File | Purpose | Setup |
|------|---------|-------|
| **CLAUDE.md** | Project context and memory | Create in project root - [See guide](docs/CLAUDE_MD_GUIDE.md) |

### 2. Globally Installed Tools

| Tool | Purpose | Installation |
|------|---------|--------------|
| Claude Code CLI | Anthropic's official CLI for Claude | `npm i -g @anthropic-ai/claude-code` |
| GitHub CLI | GitHub operations from terminal | `brew install gh` (macOS) |

### What Claude Code Can Do With These Tools

#### With GitHub CLI (`gh`)
- Create pull requests after making code changes
- Manage GitHub issues (create, list, close, comment)
- Check GitHub Actions workflow status
- Create and manage releases
- Fetch information from GitHub repositories
- Authenticate with GitHub
- Call GitHub API for custom operations

## Installation Instructions for Claude Code

When setting up on a new machine, Claude Code should install these tools in order:

### 1. Claude Code CLI (if not already installed)
```bash
npm i -g @anthropic-ai/claude-code
```

### 2. GitHub CLI
**macOS:**
```bash
brew install gh
```

**Linux (Debian/Ubuntu):**
```bash
sudo apt install gh
```

**Linux (Fedora/RHEL):**
```bash
sudo dnf install gh
```

**Windows:**
```bash
# Using winget
winget install --id GitHub.cli

# OR using Chocolatey
choco install gh
```

## Post-Installation Setup

### GitHub CLI Authentication
```bash
gh auth login
```

### Verify Installations
```bash
claude --version
gh --version
```

## Adding New Tools

When installing new tools for Claude Code:
1. Ask Claude Code to install the tool globally
2. Ask Claude Code to update [INSTALLATION_LOG.md](INSTALLATION_LOG.md) with:
   - Installation date
   - Tool name and version
   - Installation command for each platform
   - Purpose and capabilities it adds
3. Ask Claude Code to update this README with the new tool

## License

MIT