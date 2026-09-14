# The language of design

A daily design vocabulary tool. Five terms a day, each with a definition, where it came from, a practice note, a sentence you can use in a review, and search keywords for going deeper.

Block 1 of 7 is written: **70 terms across 17 days** covering design fundamentals. The remaining six blocks — UI, UX, Color, Typography, Components, Communication — are listed as a roadmap.

## Put it online

1. Create a new **public** repository on GitHub.
2. Upload `index.html`. The filename must stay exactly that.
3. **Settings → Pages → Source:** Deploy from a branch. Branch `main`, folder `/ (root)`. Save.
4. Wait about a minute. The site is at `https://YOUR-USERNAME.github.io/REPO-NAME/`

Nothing to install and nothing to build. The file runs on its own.

## How it works

- One day is visible at a time. The rest are locked until you finish the one before.
- Tick all five terms to unlock the **Finish day** button, which moves you on.
- A timer counts your time on the page against a daily goal. It pauses on demand and auto-pauses when you switch tabs.
- Search covers every day you have unlocked.
- Review days sit after every five study days.

Sequential locking, the timer, the history section, and expand-by-default can all be turned off under the gear icon.

## Progress

Day to day, progress saves to browser storage on the device you are using.

To carry it to another browser or phone, open **Settings → Save progress into a new index.html**. That downloads a copy of this file with your current progress written into it. Upload that copy to GitHub, replacing the old one, and every browser that loads the page starts from that point.

It is a manual step, not automatic sync — think of it as committing your progress rather than saving it. Once a session or once a week is enough. If two devices both study between uploads, whichever you upload last wins.

Nothing leaves your machine and there is no account.

## Editing the terms

Open `index.html` and find `const DAYS`. Each term is one object:

```js
{n:"Affordance",
 d:"One-line definition.",
 h:"Where it came from. Two to four sentences.",
 p:"How it shows up in real work.",
 s:"A sentence you could say in a review.",
 k:["search phrase one","search phrase two"]}
```

Days need `block`, `day`, `title`, `connect`, `exercise`, and a `terms` array. Review days carry `review:true` and a `reviewOf` list of day numbers instead of terms.

## Built with

No frameworks. Plain HTML, CSS and JavaScript in a single file. Two web fonts from Google Fonts (Instrument Serif for headings, Open Sans for reading), with system fallbacks if they fail to load.
