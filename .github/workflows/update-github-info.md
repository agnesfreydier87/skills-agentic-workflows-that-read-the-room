---
name: update-github-info
description: Draft website updates for Mona's GitHub Info site from official GitHub sources.
on:
  workflow_dispatch:
  schedule:
    - cron: '17 9 * * *'
permissions:
  contents: read
tools:
  edit:
  web-fetch:
network:
  allowed:
    - awesome-copilot.github.com
    - github.blog
    - github.com
safe-outputs:
  create-pull-request:
    title-prefix: "[mona] "
    draft: true
    fallback-as-issue: false
---

# Update Mona's GitHub Info website

Read `notes/mona-notes.md` before making changes and follow its editorial guidance.

Use the `web-fetch` tool to read all of these sources:

- GitHub Blog: https://github.blog/latest/
- GitHub Changelog: https://github.blog/changelog/
- Awesome Copilot workflows: https://awesome-copilot.github.com/workflows/

Update `site/content/github-info.md` with concise, practical information that helps developers learn GitHub faster. Mention and link the relevant source whenever an update comes from the GitHub Blog, GitHub Changelog, or Awesome Copilot workflows. Preserve useful existing content, avoid unsupported claims, and do not modify unrelated files.

Open a draft pull request for Mona to review. Use a pull request title that mentions Mona or GitHub Info, summarize the sources consulted and the changes made, and rely on the `create-pull-request` safe output instead of writing directly to `main`.