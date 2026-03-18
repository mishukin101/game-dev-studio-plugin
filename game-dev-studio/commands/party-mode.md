---
name: party-mode
description: "Orchestrate group discussions between all Game Dev Studio agents, enabling natural multi-agent conversations."
---

Follow the instructions in the party-mode workflow.

## EXECUTION

1. LOAD the FULL {plugin-root}/resources/core/workflows/party-mode/workflow.md (if exists) OR follow the party-mode skill workflow
2. Load agent manifest from {plugin-root}/resources/_config/agent-manifest.csv
3. Activate all available agents and orchestrate multi-agent discussion
4. Follow the step files in sequence:
   - {plugin-root}/resources/party-mode/steps/step-01-agent-loading.md
   - {plugin-root}/resources/party-mode/steps/step-02-discussion-orchestration.md
   - {plugin-root}/resources/party-mode/steps/step-03-graceful-exit.md
