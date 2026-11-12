---
name: update-github-info
description: Propose practical GitHub Info updates for Mona to review.
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
    - github.blog
    - github.com
    - awesome-copilot.github.com
engine:
  id: copilot
  copilot-sdk: true
safe-outputs:
  create-pull-request:
    title-prefix: "[mona] "
    draft: true
    fallback-as-issue: false
    allowed-files:
      - site/content/github-info.md
---

# Update Mona's GitHub Info website

Read `notes/mona-notes.md` and `site/content/github-info.md` first.
Fetch the GitHub Blog at https://github.blog/latest/, the GitHub Changelog
at https://github.blog/changelog/, and Awesome Copilot workflows at
https://awesome-copilot.github.com/.

Update `site/content/github-info.md` with relevant, concise, practical
information that helps developers learn GitHub. Include links to the original
sources and avoid repeating information already present.

If there are meaningful updates, use the `create-pull-request` safe-output to
open a pull request for Mona to review. Do not write directly to `main`.
If there are no meaningful updates, call `noop` with the reason. If a required
source cannot be fetched, report the failure rather than inventing information.
