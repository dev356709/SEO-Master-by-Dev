# SEO Master by Dev

Welcome! If you are building a website, publishing articles, or trying to grow a YouTube channel, SEO can sometimes feel like a puzzle. I built this ChatGPT skill to help creators, freelancers, and small businesses tackle SEO practically—without needing expensive subscriptions, API keys, or complicated tech setups. Just bring your content and your audience, and let's get to work!

## 🚀 What It Helps You Do

*   **Brainstorm Keywords:** Discover what your audience is actually searching for and organize those ideas by intent.
*   **Audit Your Pages:** Paste in a web page, and get a prioritized, honest list of useful SEO improvements.
*   **Write Better Metadata:** Draft catchy page titles, meta descriptions, and complete content briefs.
*   **Package YouTube Videos:** Turn your video transcripts into accurate YouTube titles, descriptions, chapter plans, and thumbnail ideas (no clickbait!).
*   **Plan Your Content:** Build a realistic content calendar and figure out how to link your pages together.
*   **Understand Your Data:** Need help reading your performance stats? It will help you interpret your numbers without inventing fake metrics.

*Note: This tool works with whatever language and niche you choose. It doesn't crawl sites automatically or guarantee overnight #1 rankings, but it gives you solid, practical steps to improve.*

## 💬 How to Try It Out

Once you have this skill loaded into ChatGPT, simply ask it for help just like you would a human assistant. Here are a few prompts you can try:

> "Review this landing page for SEO. My audience is first-time home bakers. Tell me what I can fix right now, and separate that from things you can't check."

> "Create a YouTube title, description, and thumbnail brief from this tutorial transcript. Make sure every promise is accurate."

> "Group these keyword ideas into topics for a small gardening website. I don't have search volume data, so treat these as editorial priorities."

## 🛠️ For GitHub Users & Developers

If you want to poke around the code or install this locally, go ahead and download or clone the repository (suggested folder name: `seo-master-by-dev`). Be sure to keep hidden folders like `.agents`. 

**Package Contents:**
*   `plugins/seo-master-by-dev/plugin.json`: How the plugin looks and acts.
*   `plugins/seo-master-by-dev/skills/seo-master/SKILL.md`: The core brain and main SEO instructions.
*   `docs/`, `examples/`, `tests/`: Everything you need to see how it works and check that it's running smoothly.

**Building and Checking (Optional):**
You don't need Python to use the skill in ChatGPT! But if you are modifying the repository, you can run these commands (Python 3.10+):
```bash
python3 scripts/check_package.py
python3 -m unittest discover -s tests -v
python3 scripts/build_zip.py
