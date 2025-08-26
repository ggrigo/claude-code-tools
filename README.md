# Claude Code Tools

A collection of globally installed tools that enhance Claude Code's capabilities for development workflows.

## Purpose

This project serves as:
1. Documentation of all tools installed to enhance Claude Code
2. Installation instructions for Claude Code to replicate the setup on other machines
3. A reference for Claude Code capabilities with these tools

## How to Use This Repository

Simply ask Claude Code to:
1. Read this README or INSTALLATION_LOG.md
2. Install the tools listed below using the appropriate commands for your platform
3. Claude Code will handle the installation automatically

## Installed Tools

### Core Tools

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