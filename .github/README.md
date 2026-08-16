# Platform CI reusable workflow library (LiquidMovz mirror plane)

Source of truth: `/adapt/platform/devops/platform-ci/reusable-workflows/` (Forge kit).
Mirror-plane library for `LiquidMovz/*` repos. Org-plane equivalent: `adaptnova/.github`.

| Workflow | Purpose |
|---|---|
| verify-node.yml | npm ci + gitleaks + audit + types + tests + build |
| verify-rust.yml | fmt + clippy + test + build + cargo-deny |
| verify-full.yml | combined (nova-cf pattern: node + rust + contract gates) |
| jira-key.yml | PR branch/title Jira-key guard (pull_request_target) |

Tag `v1` marks the phase1 frozen set. Promote changes via the kit, then retag.
