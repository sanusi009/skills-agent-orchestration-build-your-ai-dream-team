# Agent team

Mona's Project Pulse dashboard is built using a specialized four-agent team orchestrated through GitHub Copilot CLI in a Codespace. Each agent brings focused expertise to ensure high-quality implementation across all aspects of the application.

## Agent roles and responsibilities

### Orchestrator
- **Model**: Claude Opus 5.5 (copilot)
- **File**: `.github/agents/orchestrator.agent.md`
- **Responsibility**: Coordinates the entire team by breaking down complex requests into focused tasks and delegating work to specialist agents. Manages execution phases, prevents file conflicts, ensures parallel work runs safely, and validates that the integrated result is cohesive.

### Planner
- **Model**: Claude Opus 5.5 (copilot)
- **File**: `.github/agents/planner.agent.md`
- **Responsibility**: Creates detailed implementation strategies through thorough research of the codebase, dependencies, and edge cases. Produces ordered implementation steps, identifies file ownership, maps dependencies, and highlights validation requirements.

### Coder
- **Model**: GPT-5.5 (copilot)
- **File**: `.github/agents/coder.agent.md`
- **Responsibility**: Implements code-oriented tasks including application logic, bug fixes, and support configurations. For Project Pulse, creates launch configurations, ensures testable and deterministic behavior, and validates changes before reporting completion.

### Designer
- **Model**: Gemini 3.7 Flash (copilot)
- **File**: `.github/agents/designer.agent.md`
- **Responsibility**: Handles UI/UX, visual design, accessibility, and information architecture. For Project Pulse, ensures a polished dashboard with visible project cards, status badges, responsive layout, and clear visual affordances.

## Orchestration environment

The team operates in a GitHub Copilot CLI session within a Codespace, enabling seamless coordination, parallel task execution, and real-time feedback loops. The Orchestrator ensures no git operations occur during agent work—the learner controls all staging, commits, and pushes through explicit Copilot CLI prompts.
