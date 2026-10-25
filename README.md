# SEO-Master-by-Dev
create SEO and audit 
# SEO Master by Dev

**Practical SEO help for anyone building a website, publishing content or growing a YouTube channel.**

A skills-based plugin for ChatGPT and Codex, built for creators, freelancers, small businesses and marketing teams. Bring your own topic, audience and content. No channel-specific branding, paid SEO subscription, hosted backend or API key is required by this package.

## What it helps you do

- Discover keyword ideas and organize them by search intent.
- Review a web page and prioritize useful SEO improvements.
- Write page titles, meta descriptions and content briefs.
- Prepare YouTube titles, descriptions, thumbnail briefs and chapter plans.
- Build a realistic content calendar and internal-link plan.
- Interpret supplied performance data without inventing metrics.

It works with the language and niche you choose. Live research depends on the tools available in your ChatGPT session. Without browsing or analytics, it can improve supplied content and explain what remains unverified. It does not provide search-volume data, crawl sites automatically, guarantee rankings or publish changes.

## Try it

After installing, select **SEO Master by Dev** in the plugin picker and provide your material:

> Review this landing page for SEO. My audience is first-time home bakers. Separate observed issues from checks you cannot perform.

> Create a YouTube title, description and thumbnail brief from this tutorial transcript. Keep every promise accurate.

> Group these keyword ideas into topics for a small gardening website. I do not have search-volume data, so label priorities as editorial judgments.

For the documented local setup, see [Installation](docs/INSTALL.md). The repository contains the marketplace catalog and plugin together. If your environment does not support plugin installation, you can supply [the skill](plugins/seo-master-by-dev/skills/seo-master/SKILL.md) and its relevant reference files in a chat; that is a manual fallback, not an installed plugin.

## For GitHub users

Download or clone the repository and keep hidden folders such as `.agents`. The publisher's GitHub username has intentionally not been guessed. Suggested repository name: `seo-master-by-dev`.

This repository is ready to share as source. It has not been listed in the public ChatGPT directory. Public distribution there requires a separate submission and review; see [Publishing](docs/PUBLISHING.md).

## Package contents

```text
.agents/plugins/marketplace.json       Local repository catalog
plugins/seo-master-by-dev/
  plugin.json                         Plugin identity and display metadata
  skills/seo-master/
    SKILL.md                          Main SEO workflow
    agents/openai.yaml                Skill display metadata
    references/                       Seven focused workflows
    assets/                           Editable profile and report templates
docs/                                 Installation, publishing and validation
examples/                             Original, fictional worked examples
scripts/                              Offline validation and ZIP packaging
tests/                                Package integrity checks
LICENSE                               MIT
```

## Build and check

Python 3.10+ is only needed for repository maintenance, not for using the skill:

```sh
python3 scripts/check_package.py
python3 -m unittest discover -s tests -v
python3 scripts/build_zip.py
```

The build writes `dist/seo-master-by-dev-plugin.zip` for plugin upload and `dist/seo-master-by-dev-source.zip` for sharing this repository. The plugin ZIP has `plugin.json` at its root. No files are installed or uploaded by these commands.

## Privacy and limits

This plugin has no server, analytics beacon, account connection or data store operated by Dev. Content still goes through the host assistant and any tools you choose to use; their terms apply. Do not post private client material in public GitHub issues. See [Privacy](plugins/seo-master-by-dev/PRIVACY.md).

The instructions and examples are original and licensed under [MIT](LICENSE). The project was inspired by the modular workflow approach of [youtube-agent-skill](https://github.com/Jakeschincariol/youtube-agent-skill); none of its code or prompt text is bundled. This is an independent project, not an OpenAI or Google endorsement.
