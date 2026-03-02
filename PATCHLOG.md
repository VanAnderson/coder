# PATCHLOG

This file tracks customizations applied in `VanAnderson/coder` relative to upstream `coder/coder`.

## Custom fork changes

1. Added `.github/workflows/jarvis-sync-upstream.yml`
   - Scheduled/manual sync of `upstream-main` from upstream `coder/coder`.
2. Added `.github/workflows/jarvis-release-aws.yml`
   - On `main` pushes, mirrors `ghcr.io/coder/coder:latest` into ECR, then triggers SSM deploy command.

## Drift policy

- Keep fork changes minimal and isolated to deployment automation.
- Prefer integration via Jarvis service and Coder APIs over source modifications.
