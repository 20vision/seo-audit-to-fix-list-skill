# SEO audit to fix list (Claude skill)

Audit the pages of a website and get a spreadsheet with title, description, H1, broken links and what to fix for each page. The skill hands the job to your own MyClawn cloud computer: a real browser that stays signed in, its own email address and files. It comes back with the answer, a screenshot of the final screen and a link to a screen recording.

## Example request

> Audit the first 30 pages you can reach from <your site URL>. For each page note the title, meta description, H1, and whether any link on it is broken. Put it in a spreadsheet with a column “what to fix”.

## What you get

- It answers with a spreadsheet: one row per page, what is missing or too long, and what to change.
- A screenshot of the final screen and a link to a screen recording.

## What it does not do

- It is a reading of the pages it opens, not a crawler of thousands of URLs and not a rankings tool: it has no search-position or backlink data.
- Pages behind a login need you to sign in once on the live screen.
- It lists fixes; it does not change your site.

## Install

Claude Code, as a personal skill:

```sh
mkdir -p ~/.claude/skills/seo-audit-to-fix-list && curl -fsSL https://raw.githubusercontent.com/20vision/seo-audit-to-fix-list-skill/main/SKILL.md -o ~/.claude/skills/seo-audit-to-fix-list/SKILL.md
```

With the skills tool (installs into the current project):

```sh
npx skills add 20vision/seo-audit-to-fix-list-skill
```

## Needs

The MyClawn Computer connector, signed in with your own MyClawn account. Setup and details: https://www.myclawn.com/docs/connectors?utm_source=github&utm_medium=repo&utm_campaign=seo-audit-to-fix-list

Full description of this job, with the steps and the limits: https://www.myclawn.com/run-an-seo-audit-on-my-website?utm_source=github&utm_medium=repo&utm_campaign=seo-audit-to-fix-list

## Also listed

- https://www.skillsdirectory.com/skills/20vision-seo-audit-to-fix-list
- https://www.agensi.io/skills/seo-audit-to-fix-list
- All skills: https://github.com/20vision/skills

Made by 20Vision, the company behind MyClawn.
