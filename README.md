# EgoHackZero's Useful Tools for Claude Code

A comprehensive collection of specialized AI agents and developer tools for Claude Code that dramatically enhance productivity through intelligent automation and expert guidance.

## Overview

This extension provides 5 specialized AI agents and practical commands to supercharge your development workflow:

- **AI Agents**: Expert systems for research, learning, refactoring, architecture, and documentation
- **Commands**: Practical tools like conda environment management

## Installation

### Quick Install (Recommended)

1. **Add the marketplace:**
   ```
   /plugin marketplace add egohackzero/usefull-tools
   ```

2. **Install the plugin:**
   ```
   /plugin install egohackzero-usefull-tools
   ```

3. **Start using the agents and commands immediately!**

### Alternative: Local Development Installation

If you want to use a local copy or contribute to development:

```bash
# Clone the repository
git clone https://github.com/egohackzero/usefull-tools.git

# Add as local marketplace
/plugin marketplace add /path/to/usefull-tools

# Install the plugin
/plugin install egohackzero-usefull-tools
```

### Managing the Plugin

- **Enable:** `/plugin enable egohackzero-usefull-tools`
- **Disable:** `/plugin disable egohackzero-usefull-tools`
- **Uninstall:** `/plugin uninstall egohackzero-usefull-tools`
- **View all plugins:** `/plugin`

### Requirements

- Claude Code CLI version 2.0.0 or higher
- For `/conda-run` command: Conda/Miniconda installed with initialization script at `~/miniconda3/etc/profile.d/conda.sh`

## AI Agents

### 🔍 Deep Research Agent
**Category:** Analysis
**Trigger:** Complex investigation and research needs

Comprehensive research specialist with adaptive strategies and intelligent exploration.

**Capabilities:**
- Multi-hop reasoning with up to 5 levels of depth
- Adaptive planning strategies (simple, ambiguous, or complex queries)
- Self-reflective progress assessment and quality monitoring
- Evidence-based analysis with proper citations
- Parallel search optimization and tool orchestration

**Best For:**
- Current events and technical research
- Complex information synthesis
- Academic research contexts
- Evidence-based analysis and investigation

### 📚 Learning Guide
**Category:** Communication
**Trigger:** Code explanation and programming education

Expert programming educator focused on understanding through progressive learning and practical examples.

**Capabilities:**
- Concept breakdown with multiple explanation approaches
- Progressive skill building with prerequisite mapping
- Working code demonstrations with variations
- Educational exercises that build confidence
- Knowledge assessment and understanding verification

**Best For:**
- Teaching programming concepts
- Creating tutorials and learning paths
- Algorithm breakdowns and explanations
- Educational content design

### ♻️ Refactoring Expert
**Category:** Quality
**Trigger:** Code quality improvement and technical debt reduction

Systematic code quality improvement through proven refactoring patterns and clean code principles.

**Capabilities:**
- Complexity metric analysis (cyclomatic, maintainability index)
- SOLID principles and design pattern application
- Duplication elimination and anti-pattern removal
- Safe, incremental transformations with testing
- Before/after quality metrics and improvement tracking

**Best For:**
- Reducing code complexity and technical debt
- Applying SOLID principles and design patterns
- Improving maintainability and readability
- Safe code transformation

### 🏗️ System Architect
**Category:** Engineering
**Trigger:** System architecture design and scalability planning

Holistic system design with focus on scalability, maintainability, and long-term technical strategy.

**Capabilities:**
- Component boundary definition and dependency mapping
- Scalability architecture for 10x growth scenarios
- Architectural pattern evaluation (microservices, CQRS, event sourcing)
- Technology selection with long-term impact analysis
- Migration strategies and technical debt planning

**Best For:**
- Designing scalable system architectures
- Evaluating architectural patterns
- Technology selection and migration planning
- Creating comprehensive design documentation

### 📝 Technical Writer
**Category:** Communication
**Trigger:** Documentation creation and improvement

Clear, comprehensive technical documentation tailored to specific audiences with focus on usability.

**Capabilities:**
- Audience analysis and skill level assessment
- Information architecture and logical content structure
- Clear instructions with working examples
- WCAG accessibility compliance
- API documentation, user guides, and troubleshooting

**Best For:**
- API documentation and technical specifications
- User guides and tutorials
- Troubleshooting and installation guides
- Accessibility-compliant documentation

## Commands

### 🐍 `/conda-run [env_name]`
**Category:** Run

Seamlessly manage and run Python code with conda environments directly from Claude Code.

**Features:**
- Automatic environment detection and creation
- Smart environment selection with interactive prompts
- Support for multiple Python versions (3.10, 3.11, 3.12)
- Integrated package installation (pip/conda)
- Persistent environment activation

**Usage:**
```bash
# Run with specific environment
/conda-run ml-project

# Interactive selection
/conda-run
```

## Agent Categories

- **Analysis**: `deep-research-agent`
- **Communication**: `learning-guide`, `technical-writer`
- **Quality**: `refactoring-expert`
- **Engineering**: `system-architect`

## Use Cases

### Research & Learning
- Investigate complex technical topics with Deep Research Agent
- Learn new programming concepts with Learning Guide
- Create comprehensive documentation with Technical Writer

### Code Quality
- Refactor legacy code with Refactoring Expert
- Design new systems with System Architect
- Reduce technical debt systematically

### Development Workflow
- Manage Python environments with `/conda-run`
- Generate API documentation with Technical Writer
- Plan architectural changes with System Architect

## Contributing

Contributions are welcome! To add new agents or commands:

1. Fork the repository
2. Create your agent in `.claude/agents/` or command in `.claude/commands/`
3. Update `.claude-plugin/plugin.json` with the new agent/command metadata
4. Submit a pull request

### Agent Structure
```markdown
---
name: agent-name
description: Brief description
category: analysis|communication|quality|engineering
---
# Agent content
```

## License

MIT License - See LICENSE file for details

## Author

**egohackzero**

## Changelog

### v1.0.0 (Initial Release)
- 5 specialized AI agents: Deep Research, Learning Guide, Refactoring Expert, System Architect, Technical Writer
- `/conda-run` command for conda environment management
- Comprehensive documentation and examples
- Full agent categorization system
