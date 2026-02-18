# GitHub Copilot Instructions

This repository is the **root planning and governance repo** for Server Orchestrator.
Use it for project coordination, documentation, policy, and product vision.

## Repository Scope

Prefer changes in this repository for:
- GitHub Projects setup and workflow definitions
- Initiative, epic, and issue planning
- Product and technical vision documents
- Policies, standards, and team process docs
- Cross-repository coordination docs

Avoid placing implementation-specific application code here unless explicitly requested.

## Project Context

Server Orchestrator is a Kubernetes-first platform to operate containerized game servers with:
- Multi-tenant namespace isolation
- Template-driven server provisioning
- Namespace RBAC and controlled delegation
- Resource and file management workflows
- Unified UI and API for operators and automation

This root repo represents the program-level source of truth for direction and coordination.

## How Copilot Should Assist Here

When creating or editing content in this repo:
1. Prioritize clarity, decision traceability, and actionable outcomes
2. Prefer structured Markdown (headings, concise bullet lists, explicit next steps)
3. Separate strategy from execution details
4. Reference affected component repos when work is implementation-specific
5. Keep language precise and policy-aligned; avoid vague statements

## Issue and Planning Guidance

When drafting issues:
- Include clear problem statement, desired outcome, and scope boundaries
- Add concrete acceptance criteria
- Call out dependencies, risks, and out-of-scope items
- Distinguish strategic work (vision/policy) from delivery work (feature/task)

When drafting epics or initiatives:
- Define objective, success metrics, and milestone checkpoints
- Break work into trackable child issues
- Document cross-repo impact (for example API, backend, frontend, infra)

## Documentation and Policy Guidance

When drafting docs:
- Prefer normative wording for policy content (`must`, `should`, `may`)
- Include rationale for non-obvious constraints
- Add ownership and review expectations when relevant
- Keep documents durable and not tied to temporary implementation details

## Cross-Repository Coordination

For work that belongs in another repository:
- Do not invent code changes in this repo
- Propose the target repository and affected area
- Provide issue-ready implementation guidance that can be transferred
- Keep this repo focused on orchestration of work, not application code

## Quality Bar

Content produced in this repository should be:
- Specific and testable (especially acceptance criteria and policies)
- Consistent with the Server Orchestrator vision and domain model
- Minimal but complete, avoiding filler text
- Easy to convert into GitHub issues, project items, and roadmap updates
