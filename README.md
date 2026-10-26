<div align="center">
    <h1>🤖 Awesome OpenCode CLI Subagents</h1>
    <p><strong>A curated collection of specialized AI assistants for OpenCode CLI</strong></p>
    <br />
</div>

<div align="center">

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
![Subagent Count](https://img.shields.io/badge/subagents-175-blue?style=flat-square)
[![Last Update](https://img.shields.io/github/last-commit/ankitmundada/awesome-opencode-subagents?label=Last%20update&style=flat-square)](https://github.com/ankitmundada/awesome-opencode-subagents)

</div>

<br />

# Awesome OpenCode CLI Subagents

This repository serves as the definitive collection of OpenCode CLI subagents, specialized AI assistants designed for specific development tasks.

## Installation

### Option 1: Manual Installation (Recommended)

1. Clone this repository
2. Copy desired agent files to:
   - `~/.config/opencode/agents/` for global access
   - `.opencode/agents/` for project-specific use
3. Customize based on your project requirements

### Option 2: Interactive Installer

```bash
git clone https://github.com/ankitmundada/awesome-opencode-subagents.git
cd awesome-opencode-subagents
./install-agents.sh
```

This interactive script lets you browse categories, select agents, and install/uninstall them with a single command.

### Option 3: Standalone Installer (no clone required)

```bash
curl -sO https://raw.githubusercontent.com/ankitmundada/awesome-opencode-subagents/main/install-agents.sh
chmod +x install-agents.sh
./install-agents.sh
```

Downloads agents directly from GitHub without cloning the repository. Requires `curl`.

## 📚 Categories

Check the [categories/](categories/) directory for the full list of available subagents.

## 🤖 Understanding Subagents

Subagents are specialized AI assistants that enhance OpenCode CLI's capabilities by providing task-specific expertise. They act as dedicated helpers that OpenCode CLI can call upon when encountering particular types of work.

### Subagent Storage Locations

| Type              | Path                        | Availability         | Precedence |
| ----------------- | --------------------------- | -------------------- | ---------- |
| Project Subagents | `.opencode/agents/`         | Current project only | Higher     |
| Global Subagents  | `~/.config/opencode/agents/`| All projects         | Lower      |

Note: When naming conflicts occur, project-specific subagents override global ones.

## 📖 Subagent Structure

Each subagent follows a standardized template:

```markdown
---
description: When this agent should be invoked
mode: subagent
tools:
  write: true
  edit: true
  bash: true
temperature: 0.1
steps: 20
---

You are a [role description and expertise areas]...

[Agent-specific checklists, patterns, and guidelines]...

## Communication Protocol
Inter-agent communication specifications...

## Development Workflow
Structured implementation phases...
```

## 🤝 Contributing

We welcome contributions! See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

- Submit new subagents via PR
- Improve existing definitions
- Report issues and bugs

## 📄 License

MIT License - see [LICENSE](LICENSE)
