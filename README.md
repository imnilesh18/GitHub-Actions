# GitHub Actions — Containers, Custom Actions, and Security

A hands‑on repo exploring GitHub Actions end to end: run jobs in containers, spin up service containers, build custom actions (Composite, JavaScript, Docker), deploy with a JS action, and harden workflows with least‑privilege permissions and safe patterns.

## What’s inside

- Containers for Jobs
  - Run jobs in containerized environments (e.g., node:16)
  - Keep workflows reproducible and portable

- Service Containers
  - Ephemeral services alongside jobs (e.g., MongoDB for tests)
  - Container networking and port mapping examples

- Custom Actions
  - Composite Action: reusable deps cache + install
    - Inputs: toggle caching
    - Outputs: expose cache usage
  - JavaScript Action: log + deploy example
  - Docker Action: containerized logic blueprint

- Deployment Demo
  - JavaScript action scaffolding a static site upload to S3

- Security Essentials
  - Script Injection: demo + mitigation with env vars
  - Using Actions Securely: verified creators, review code, or build your own
  - Permissions: least‑privilege on jobs/workflows
  - GITHUB_TOKEN: short‑lived token scoped by permissions
  - Repo Settings: PR approvals from forks, allowed actions, PR auto‑approve toggle

## Quick start

1. Clone and open the workflows in `.github/workflows`
2. Explore local actions in `.github/actions/`
3. Push to trigger the pipelines and see jobs, services, and custom actions in action

## Highlights

- DRY workflows via a composite action that caches and installs dependencies
- Configurable inputs/outputs for reuse across lint/test/build
- Containerized testing with a MongoDB service
- Minimal, readable examples focused on core concepts

## Why this repo

- Learn by example with concise, production‑flavored patterns  
- Copy/paste friendly snippets to bootstrap real CI/CD  
- Security baked in: defaults that nudge toward safer pipelines

## License

[MIT license](LICENSE)

