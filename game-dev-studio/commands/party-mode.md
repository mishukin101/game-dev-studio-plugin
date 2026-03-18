---
name: party-mode
description: "모든 Game Dev Studio 에이전트 간의 그룹 토론을 조율하는 멀티 에이전트 대화를 시작합니다."
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
