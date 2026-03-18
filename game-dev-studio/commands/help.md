---
name: help
description: "Game Dev Studio 워크플로우에서 다음 단계를 분석하고 안내합니다."
---

# Task: Game Dev Studio Help

## ROUTING RULES

- **Empty `phase` = anytime** — Universal tools work regardless of workflow state
- **Numbered phases indicate sequence** — Phases flow in order
- **Stay in module** — Guide through the active module's workflow based on phase+sequence ordering
- **`required=true` blocks progress** — Required workflows must complete before proceeding

## EXECUTION

1. **Load catalog** — Load `{plugin-root}/resources/_config/bmad-help.csv`
2. **Resolve output locations and config** — Scan each folder under `{plugin-root}/resources/` (except `_config`) for `config.yaml`. Resolve `output-location` variables against that module's config. Extract `communication_language` and `project_knowledge`.
3. **Ground in project knowledge** — If `project_knowledge` resolves to an existing path, read available documentation.
4. **Detect active module** — Use conversation context
5. **Analyze input** — Infer what was just completed
6. **Present recommendations** — Show next steps based on completed workflows, phase/sequence ordering, and artifact presence
7. Present all output in `{communication_language}`
