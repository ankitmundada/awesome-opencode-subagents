# LLMOps, Evals & Observability Subagents

LLMOps, Evals & Observability subagents help teams evaluate AI systems, investigate output quality, and operate LLM and agent workflows with production-grade telemetry.

## When to Use LLMOps, Evals & Observability Subagents

Use these subagents when you need to:
- **Design evaluations** for AI workflows
- **Detect prompt or model regressions**
- **Investigate hallucinations** and unsupported claims
- **Instrument production AI systems** with useful signals

## Available Subagents

### [**ai-observability-engineer**](ai-observability-engineer.md) - AI observability engineer
Designs AI-native traces, metrics, logging, and debugging signals for production LLM and agent systems.

**Use when:** Instrumenting or debugging production AI behavior.

### [**eval-engineer**](eval-engineer.md) - AI evaluation engineer
Designs evaluations for prompts, retrieval, tools, and multi-step agent workflows.

**Use when:** Establishing quality measurement for an AI system.

### [**hallucination-investigator**](hallucination-investigator.md) - AI hallucination investigator
Performs root-cause analysis for factuality failures, unsupported claims, and context breakdowns.

**Use when:** Investigating why an AI output was inaccurate or unsupported.

### [**prompt-regression-tester**](prompt-regression-tester.md) - AI regression testing specialist
Builds regression coverage for prompt, model, tool, and workflow changes.

**Use when:** Validating that an AI system change has not degraded quality.

## Quick Selection Guide

| If you need to... | Use this subagent |
|-------------------|-------------------|
| Instrument production AI systems | **ai-observability-engineer** |
| Design AI evaluations | **eval-engineer** |
| Investigate hallucinations | **hallucination-investigator** |
| Test AI changes for regressions | **prompt-regression-tester** |
