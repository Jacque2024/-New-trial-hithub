# Graph Report - -New-trial-hithub  (2026-10-12)

## Corpus Check
- Corpus is ~3,579 words - fits in a single context window. You may not need a graph.

## Summary
- 36 nodes · 76 edges · 6 communities
- Extraction: 70% EXTRACTED · 30% INFERRED · 0% AMBIGUOUS · INFERRED: 23 edges (avg confidence: 0.87)
- Token cost: 74,803 input · 0 output

## Community Hubs (Navigation)
- Course Setup & Codespaces
- Copilot Concepts & Features
- Step 2 JavaScript Function
- Step 4 Comment Codegen
- Step 3 Copilot Hub
- Step 1 Devcontainer Check

## God Nodes (most connected - your core abstractions)
1. `Code with GitHub Copilot (course README)` - 10 edges
2. `GitHub Copilot` - 9 edges
3. `Step 1: Leverage Codespaces with VS Code for Copilot` - 8 edges
4. `Step 4: Using comments to generate code` - 7 edges
5. `on_add_devcontainer job` - 7 edges
6. `on_functionadded job` - 7 edges
7. `on_copilothubsuggestions job` - 7 edges
8. `on_push_to_comments job` - 7 edges
9. `Step 3: Copilot tab with multiple suggestions` - 6 edges
10. `Finish: course recap and resources` - 6 edges

## Surprising Connections (you probably didn't know these)
- `Code with GitHub Copilot (course README)` --semantically_similar_to--> `Step 1: Leverage Codespaces with VS Code for Copilot`  [INFERRED] [semantically similar]
  README.md → .github/steps/1-copilot-extension.md
- `Dependabot Config (github-actions, devcontainers monthly)` --references--> `.devcontainer/devcontainer.json`  [INFERRED]
  .github/dependabot.yml → README.md
- `on_add_devcontainer job` --references--> `Code with GitHub Copilot (course README)`  [INFERRED]
  .github/workflows/1-copilot-extension.yml → README.md
- `on_functionadded job` --references--> `Code with GitHub Copilot (course README)`  [INFERRED]
  .github/workflows/2-skills-javascript.yml → README.md
- `on_copilothubsuggestions job` --references--> `Code with GitHub Copilot (course README)`  [INFERRED]
  .github/workflows/3-copilot-hub.yml → README.md

## Import Cycles
- None detected.

## Hyperedges (group relationships)
- **Copilot course step-gated progression via workflows** — _github_workflows_0_welcome_workflow, _github_workflows_1_copilot_extension_workflow, _github_workflows_2_skills_javascript_workflow, _github_workflows_3_copilot_hub_workflow, _github_workflows_4_copilot_comment_workflow, _github_steps__step_current_step_counter, _github_workflows_0_welcome_action_update_step [EXTRACTED 1.00]
- **Learner-created files validated by action-check-file** — readme_devcontainer_json, _github_steps_2_skills_javascript_skills_js, _github_steps_3_copilot_hub_member_js, _github_steps_4_copilot_comment_comments_js, _github_workflows_1_copilot_extension_action_check_file [EXTRACTED 1.00]

## Communities (6 total, 0 thin omitted)

### Community 0 - "Course Setup & Codespaces"
Cohesion: 0.33
Nodes (10): Dependabot Config (github-actions, devcontainers monthly), Step 0: Welcome placeholder, Step 1: Leverage Codespaces with VS Code for Copilot, get_current_step job, on_start job, Step 0, Welcome workflow, Code with GitHub Copilot (course README), .devcontainer/devcontainer.json (+2 more)

### Community 1 - "Copilot Concepts & Features"
Cohesion: 0.39
Nodes (7): Copilot Completions Panel, member.js (skillsMember), Step 3: Copilot tab with multiple suggestions, Step 4: Using comments to generate code, Finish: course recap and resources, GitHub Copilot, OpenAI Codex

### Community 2 - "Step 2 JavaScript Function"
Cohesion: 0.60
Nodes (5): skills.js (calculateNumbers), Step 2: AI code suggestions in a JavaScript file, get_current_step job, on_functionadded job, Step 2, Javascript function workflow

### Community 3 - "Step 4 Comment Codegen"
Cohesion: 0.50
Nodes (5): comments.js (Create web server), skills/action-update-step@v2, get_current_step job, on_push_to_comments job, Step 4, Add Copilot suggestion from comment workflow

### Community 4 - "Step 3 Copilot Hub"
Cohesion: 0.67
Nodes (4): Current Step Counter (-step.txt), get_current_step job, on_copilothubsuggestions job, Step 3, Copilot hub suggestion workflow

### Community 5 - "Step 1 Devcontainer Check"
Cohesion: 0.67
Nodes (4): skills/action-check-file@v1, get_current_step job, on_add_devcontainer job, Step 1, Copilot Extension in a Codespace workflow

## Knowledge Gaps
- **2 isolated node(s):** `Step 0: Welcome placeholder`, `OpenAI Codex`
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 2 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `Code with GitHub Copilot (course README)` connect `Course Setup & Codespaces` to `Copilot Concepts & Features`, `Step 2 JavaScript Function`, `Step 4 Comment Codegen`, `Step 3 Copilot Hub`, `Step 1 Devcontainer Check`?**
  _High betweenness centrality (0.213) - this node is a cross-community bridge._
- **Are the 6 inferred relationships involving `Code with GitHub Copilot (course README)` (e.g. with `on_start job` and `on_add_devcontainer job`) actually correct?**
  _`Code with GitHub Copilot (course README)` has 6 INFERRED edges - model-reasoned connections that need verification._
- **What connects `Step 0: Welcome placeholder`, `OpenAI Codex` to the rest of the system?**
  _2 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Why does `GitHub Copilot` connect `Copilot Concepts & Features` to `Course Setup & Codespaces`, `Step 2 JavaScript Function`?**
  _High betweenness centrality (0.170) - this node is a cross-community bridge._
- **Are the 4 inferred relationships involving `Step 1: Leverage Codespaces with VS Code for Copilot` (e.g. with `Finish: course recap and resources` and `on_start job`) actually correct?**
  _`Step 1: Leverage Codespaces with VS Code for Copilot` has 4 INFERRED edges - model-reasoned connections that need verification._
- **Why does `on_start job` connect `Course Setup & Codespaces` to `Step 4 Comment Codegen`?**
  _High betweenness centrality (0.127) - this node is a cross-community bridge._
- **Are the 3 inferred relationships involving `Step 4: Using comments to generate code` (e.g. with `Finish: course recap and resources` and `on_copilothubsuggestions job`) actually correct?**
  _`Step 4: Using comments to generate code` has 3 INFERRED edges - model-reasoned connections that need verification._