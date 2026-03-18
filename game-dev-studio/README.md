# Game Dev Studio Plugin

AI-powered game development workflow plugin for **Claude Cowork** and **Claude Code**.

Provides specialized agents, collaborative workflows, and review tools for end-to-end game development — from brainstorming to shipping.

## Agents (Skills)

Auto-activated based on task context:

| Agent | Persona | Expertise |
|-------|---------|-----------|
| Game Architect | Cloud Dragonborn | Systems architecture, engine design, multiplayer |
| Game Designer | Samus Shepard | Mechanics, player psychology, narrative design |
| Game Developer | Link Freeman | Unity, Unreal, Godot implementation |
| Game QA | GLaDOS | Test automation, performance profiling |
| Scrum Master | Max | Sprint planning, story creation, team coordination |
| Solo Dev | Indie | End-to-end indie development, Quick Flow |
| Tech Writer | Paige | Documentation, CommonMark, API docs |
| BMad Master | BMad Master | Workflow orchestration, system navigation |

## Commands (Slash Commands)

### Game Development Workflows
- `/game-dev-studio:create-game-brief` — Define game vision through collaborative discovery
- `/game-dev-studio:create-gdd` — Create comprehensive Game Design Document (24 game types supported)
- `/game-dev-studio:quick-spec` — Engineer implementation-ready technical specifications
- `/game-dev-studio:quick-dev` — Execute development tasks from specs or direct instructions
- `/game-dev-studio:generate-project-context` — Generate AI-optimized project context file

### Creative & Collaboration
- `/game-dev-studio:brainstorm` — Facilitate brainstorming with diverse creative techniques
- `/game-dev-studio:party-mode` — Multi-agent group discussion with all agents
- `/game-dev-studio:advanced-elicitation` — Push LLM to refine and improve output

### Review & Quality
- `/game-dev-studio:review-adversarial` — Cynical review finding at least 10 issues
- `/game-dev-studio:review-edge-cases` — Exhaustive path enumeration for unhandled cases
- `/game-dev-studio:review-prose` — Clinical copy-editing for communication clarity
- `/game-dev-studio:review-structure` — Structural editing for document organization

### Utilities
- `/game-dev-studio:help` — Workflow navigation and next-step guidance
- `/game-dev-studio:index-docs` — Generate folder index documentation
- `/game-dev-studio:shard-doc` — Split large documents into organized sections

## Supported Game Types (GDD)

Action Platformer, Adventure, Card Game, Fighting, Horror, Idle/Incremental, Metroidvania, MOBA, Party Game, Puzzle, Racing, Rhythm, Roguelike, RPG, Sandbox, Shooter, Simulation, Sports, Strategy, Survival, Text-Based, Tower Defense, Turn-Based Tactics, Visual Novel

## Supported Engines

- Unity
- Unreal Engine
- Godot
- Web-based / Custom

## Installation

### Claude Cowork (Desktop App)
Install from the plugin marketplace or manually:
```bash
claude plugin install game-dev-studio@your-org/game-dev-studio-plugin
```

### Claude Code (CLI / VS Code)
```bash
claude plugin marketplace add your-org/game-dev-studio-plugin
claude plugin install game-dev-studio
```

## Configuration

After installation, the plugin reads configuration from `resources/gds/config.yaml`. Key settings:

- `communication_language` — Language for agent communication (default: Korean)
- `document_output_language` — Language for generated documents
- `primary_platform` — Target game engine(s)
- `game_dev_experience` — User experience level

## Architecture

Built on the [BMAD Method](https://github.com/bmad-code-org/bmad-method) platform:

- **Micro-file architecture** — Step files loaded Just-In-Time to prevent context bloat
- **Sequential enforcement** — Disciplined step-by-step execution with user control
- **State tracking** — YAML frontmatter tracks progress with continuation support
- **Collaborative discovery** — Agents facilitate, users decide

## Attribution

This plugin is built on the [BMAD Method](https://github.com/bmad-code-org/bmad-method) platform and includes components from [bmad-module-game-dev-studio](https://github.com/bmad-code-org/bmad-module-game-dev-studio) by BMad Code, LLC.

## License

MIT License — see [LICENSE](../LICENSE) for details.

BMad™, BMAD-CORE™, BMAD-METHOD™ are trademarks of BMad Code, LLC.
