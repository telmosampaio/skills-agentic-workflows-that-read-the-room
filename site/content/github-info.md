# GitHub Info

## Mona's editorial angle

Mona's website focuses on practical GitHub guidance backed by official references from:

- docs.github.com
- github.blog
- github.blog/changelog

## Current homepage themes

- GitHub collaboration basics: repositories, branches, pull requests, and merges.
- GitHub Copilot as an AI coding assistant across the IDE, CLI, and GitHub.
- GitHub Actions as the automation layer behind repository workflows.
- Recent GitHub Blog and Changelog stories worth watching.

## Recent updates (November 2026)

### GitHub Changelog

- **Plan for `pull_request_target` changes.** From December 2, 2026, GitHub Actions blocks `pull_request_target` by default in public repositories unless an Actions event policy allows it. Private and internal repositories are not affected. Review your workflows now. ([Changelog](https://github.blog/changelog/2026-11-02-pull_request_target-blocked-by-default-december-2))
- **Track issues with statuses.** Issue statuses go beyond open/closed, and repository boards visualize them. Both are in public preview. ([Changelog](https://github.blog/changelog/2026-11-23-issue-statuses-and-repository-boards-are-in-public-preview))
- **Stop polling in scripts.** `gh event listen` (GitHub CLI v2.105.0) waits for pull request events such as reviews, check suites, and merge conflicts. ([Changelog](https://github.blog/changelog/2026-11-18-wait-for-pull-request-events-with-github-cli))
- **Catch secrets earlier.** Copilot's security review can now run secret scanning on code changes in Copilot CLI, the Copilot app, and code review (public preview, opt-in). ([Changelog](https://github.blog/changelog/2026-11-17-secret-scanning-on-demand-for-developers-and-agents))

### GitHub Blog

- [Build once, run on any agent: A practical guide to agent skills](https://github.blog/ai-and-ml/github-copilot/build-once-run-on-any-agent-a-practical-guide-to-agent-skills/)
- [Beyond code generation: A developer's guide to agentic engineering](https://github.blog/ai-and-ml/github-copilot/beyond-code-generation-a-developers-guide-to-agentic-engineering/)
- [How to continue a GitHub Copilot app session in VS Code](https://github.blog/ai-and-ml/github-copilot/how-to-continue-a-github-copilot-app-session-in-vs-code/)

### Community resources

- [Awesome GitHub Copilot](https://awesome-copilot.github.com/) is a community library of agents, instructions, skills, hooks, and [workflows](https://github.com/github/awesome-copilot/tree/main/workflows), with a Learning Hub of hands-on guides. Good starting point for agentic workflow ideas.
