# How to edit your site (no coding needed)

Do everything on github.com in your `albinawrobel.github.io` repository. To edit a file, click it, then click the pencil icon. When you're done, click **Commit changes**. The live site updates in about 1–2 minutes.

## Your details: `_config.yml`
Your name, tagline, email, booking link and social links all live here. Change the lines marked `<-- EDIT`.

## Your home page: `index.md`
Your intro, the GTM loop, what you help with and your story all live here. Edit the text between the tags; leave the `<...>` parts alone.

## Write a new article
1. Open the `_posts` folder.
2. Click **Add file → Create new file**.
3. Name it `YYYY-MM-DD-short-title.md`, for example `2026-12-01-the-mentor-feedback-trap.md`.
   - The words in the name become the web address: `/resources/the-mentor-feedback-trap/`. Use keywords people would search for.
4. Paste this at the very top, then write your article underneath in Markdown:

```
---
layout: post
title: "Your headline here"
description: "One sentence summary. Shows in Google results."
---
```

5. Commit. The article appears on your Home and Resources pages automatically.

## Write a new guide
Guides are short, step-by-step pieces (under about 5 minutes). Make one exactly like an article, in the `_posts` folder, but add `type: guide` to the top:

```
---
layout: post
type: guide
title: "Your headline here"
description: "One sentence summary. Shows in Google results."
---
```

It shows under **Guides** on the Resources page instead of Articles.

## How the Resources page fills itself
- Each section (Guides, Articles, Tools) shows your 3 newest pieces.
- Once a section has more than 3, an "Explore all →" link appears that opens the full list (`/resources/guides/`, `/resources/articles/`, `/resources/tools/`).
- A section with nothing in it shows a "coming soon" card.

Delete the sample article (`_posts/2026-11-22-article-template.md`) once you've published a real one.

## Add a new calculator or tool
Copy `tools/roi-calculator.html`, give it a new name, and change the `title`, `description` and `permalink` at the top. Keep `tool: true` so it's listed automatically. (Ask Claude to build the next one for you.)

## Markdown cheat sheet
- `## Heading`, `### Smaller heading`
- `**bold**`, `*italic*`
- `[link text](https://...)`
- `- bullet`
- `> quote`
- Three backticks ``` above and below a code block
