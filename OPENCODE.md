# OPENCODE.md

This file provides guidance to OpenCode CLI when working with code in this repository.

## Project Overview

This is a curated collection of OpenCode CLI subagent definitions - specialized AI assistants for specific development tasks. Subagents are markdown files with YAML frontmatter that OpenCode CLI can load and use.

## Repository Structure

```
categories/
  01-core-development/     # Backend, frontend, fullstack, mobile, etc.
  02-language-specialists/ # Language/framework experts (TypeScript, Python, etc.)
  03-infrastructure/       # DevOps, cloud, Kubernetes, etc.
  04-quality-security/     # Testing, security auditing, code review
  05-data-ai/              # ML, data engineering, AI specialists
  06-developer-experience/ # Tooling, documentation, DX optimization
  07-specialized-domains/  # Blockchain, IoT, fintech, gaming
  08-business-product/     # Product management, business analysis
  09-meta-orchestration/   # Multi-agent coordination
  10-research-analysis/    # Research and analysis specialists
  11-ai-governance-safety/ # AI governance, risk, and safety controls
  12-platform-engineering-idp/ # Internal developer platforms and self-service
  13-llmops-evals-observability/ # LLM evaluation, monitoring, and quality
```

## Subagent File Format

Each subagent follows this template:

```markdown
---
description: When this agent should be invoked
mode: subagent
tools:
  write: true
  edit: true
  bash: true
---

You are a [role description]...

[Agent-specific checklists, patterns, guidelines]

## Communication Protocol
[Inter-agent communication specs]

## Development Workflow
[Structured implementation phases]
```

## Subagent Storage in OpenCode CLI

| Type    | Path                        | Scope                |
| ------- | --------------------------- | -------------------- |
| Project | `.opencode/agents/`         | Current project only |
| Global  | `~/.config/opencode/agents/`| All projects         |

Project subagents take precedence over global ones with the same name.
