# Quorum

**Every pitch deserves a skeptic.** Quorum is an AI investment committee: six AI agents cross-examine a stock pitch and return a one-page decision memo.

This is our class prototype for *AI Use Case Deep Dive & Application Demo* (NYU Stern). The demo replays a recorded committee run on a hypothetical Expedia pitch. The scenario math (prices, expected return, probability edits) runs live in code.

## See it
- **Live site:** turn on GitHub Pages (see below), then use the link it gives you.
- **Locally:** download `index.html` and double-click it.

## The whole site is one file
Everything lives in `index.html`: styles at the top, page content in the middle, scripts at the bottom. There's nothing to install and no build step.

| To change… | Search `index.html` for… |
|---|---|
| Headline and hero text | `Every pitch deserves` |
| The particle number and its captions | `const SHAPES` |
| Sections on the home page | `id="committee"`, `id="how"`, `id="features"`, `id="proof"` |
| The Expedia example inputs | `const EX =` |
| The recorded agent outputs shown in the demo | `const DEMO =` |
| How long each agent "thinks" in the demo | `fact: 7200` |
| The scenario calculator | `function computeScenarios` |
| Colors and fonts | `:root {` (the first lines of the file) |

## Editing on github.com (no setup)
1. Open `index.html` and click the pencil icon (**Edit**).
2. Use Ctrl+F / Cmd+F to find what you want to change (see the table above).
3. Click **Commit changes** and write a short note about what you changed.
4. The live site updates about a minute later.

## Editing on your computer
```bash
git clone <this repo's URL>
cd quorum-ai-investment-committee
# edit index.html, then open it in a browser to check
git add index.html
git commit -m "Describe your change"
git pull --rebase   # pick up teammates' changes first
git push
```

## Rules so we don't overwrite each other
- **Pull before you edit** (or refresh the page on github.com) so you start from the latest version.
- **Keep edits small** and commit them often.
- **Say what you're changing** in the group chat if it's a big section.
- **Before you commit:** open the page in a browser and click **Run the demo** to make sure it still works.

## Turn on the free live site (one time, repo owner)
**Settings → Pages → Build and deployment → Source: Deploy from a branch → Branch: `main`, folder `/ (root)` → Save.**
After about a minute, the page shows your link: `https://jamiestuartv.github.io/quorum-ai-investment-committee/`.

---
Class prototype. Not investment advice.
