# backofthenapkin.tech
Back of the Napkin is a practitioner's sketchpad by Wayne Kirk Schmidt.
Contemplation on problems, solutions, and change.
The site is intentionally built as a **lightweight static site** with no CMS, no build step, and no dependencies beyond a browser.

---

## Important Documentation

- [OVERVIEW](/README.md)  
  This document. General overview of the site structure and how to add content.
- [TEMPLATE](posts/template.md)  
  The blank post template. Copy this to start a new article.
- [CONTRIBUTING](doc/CONTRIBUTING.md)  
  How to write, format, and publish a post.
- [DESIGN](doc/DESIGN.md)  
  Design system reference. Colors, typography, and layout decisions.

## Design Principles

- **KISS** — Keep it simple. One HTML file. One CSS file. One markdown file per post.
- **Content first** — Every post is a plain markdown file. No HTML to write. No CMS to log into.
- **Portable** — The repo is the archive. Every post is readable on GitHub without a browser.
- **Consistent** — Every post follows the same template. Same voice. Same structure.

---

## Repository Layout

```
.
├── README.md
├── background.png
├── index.html
├── styles.css
├── post.html
├── post.css
├── doc
│   ├── CONTRIBUTING.md
│   └── DESIGN.md
└── posts
    ├── template.md
    ├── incoming
    │   └── (drafts go here)
    └── 20260514.001.md
```

---

## Adding a Post

This project intentionally does **not** require a build step or deployment pipeline.

### Requirements

- A text editor
- A GitHub account
- That is it

### Steps

1. Copy `posts/template.md` to `posts/incoming/YYYYMMDD.NNN.md`
2. Fill in the frontmatter and write the post
3. When ready to publish, move the file from `posts/incoming/` to `posts/`
4. Update the post list in `index.html`
5. Done

---

## Post Template

Every post uses the same frontmatter and section structure:

```markdown
---
title: 
date: YYYY-MM-DD
id: YYYYMMDD.001
type: insight | code | research
topic: devops | ml-ai | security | practice
tagline: 
---

## Here's the thing.

## Why we care.

## What we could do.

## What the outcome was.

## What I learned.

## Make it better.
```

---

## Post Types

| Type | Structure |
|------|-----------|
| insight | Here's the thing. Why we care. What we could do. What the outcome was. What I learned. Make it better. |
| code | Collect. Organize. Determine. Evolve. What I learned. Make it better. |
| research | Goals. Context. Results. What the outcome was. What I learned. Make it better. |

## Post Topics

| Topic | Description |
|-------|-------------|
| devops | Platform engineering, CI/CD, observability, infrastructure |
| ml-ai | Machine learning, AI systems, edge inference, ethics |
| security | Zero trust, resilience, compliance, adaptive defense |
| practice | Practitioner philosophy, methodology, leadership, change |

---

## File Naming

Posts follow a date-based naming convention:

```
YYYYMMDD.NNN.md
```

Where `NNN` is a zero-padded sequence number for that day. For example:

```
20260514.001.md
20260514.002.md
```

---

## To Do

- Wire up `incoming/` as a GitHub Actions workflow to auto-publish on merge
- Add RSS feed generation
- Add search across posts
- Add related posts to post template

---

## License

Copyright 2026  
Wayne Kirk Schmidt (wayne.kirk.schmidt@gmail.com)

Licensed under the Apache 2.0 License (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    license-name   Apache 2.0
    license-url    https://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

---

## Support

Feel free to e-mail me with issues to:

- wayne.kirk.schmidt@gmail.com

Or drop a comment in the **Make it better** section of any post.
I will provide best effort responses and keep the thinking going.
