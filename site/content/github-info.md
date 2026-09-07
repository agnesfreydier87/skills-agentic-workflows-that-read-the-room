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

## Ready-made Copilot agentic workflows

The [Awesome Copilot workflows collection](https://awesome-copilot.github.com/workflows/) publishes example `gh-aw` (GitHub Agentic Workflows) configurations that developers can copy into their own repos. Highlights worth learning from:

- **Daily Issues Report** — a scheduled workflow that summarizes new, closed, and stale issues into a daily GitHub issue, so teams get a lightweight triage digest without manual effort.
- **Relevance Check** — a `/relevance-check` slash command that has Copilot review an issue or PR against the current codebase and comment on whether it's still relevant, already resolved, or superseded.
- **OSPO Stale Repository Report** — a monthly scan across an organization's repos that flags inactive ones (configurable inactivity window, exemptions by name or topic) and files/updates a report issue.
- Other workflows in the collection cover contributor reporting, org health checks, release compliance, and syncing weekly comments — useful patterns for open-source program offices (OSPO) and maintainers automating repo hygiene.

These are a good starting point if you want to add automation to a repository using GitHub Copilot's agentic workflow engine: browse the full list at [awesome-copilot.github.com/workflows](https://awesome-copilot.github.com/workflows/).

## A note on freshness

This update could not reach github.blog/latest/ or github.blog/changelog/ from the current environment (outbound web fetches were blocked), so no new Blog or Changelog items are summarized here this round. The Awesome Copilot workflows section above was verified directly against the [github/awesome-copilot](https://github.com/github/awesome-copilot) repository. Mona: please re-run this update when blog access is available to keep the "Recent GitHub Blog and Changelog stories" theme current.
