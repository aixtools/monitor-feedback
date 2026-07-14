# Monitor — feedback

**This repository is for feedback and bug reports. It holds no code.**
The only thing open here is **[Issues](../../issues)** — that is deliberate.

If something in Monitor is wrong, confusing, missing, or just annoying: open an issue.

**Prefer to talk? → [Discord](https://discord.gg/rybEwArwch)**
Good for questions, "is this just me?", and anything you would rather not post in public.
An issue is still better for a real bug — it does not scroll away.

---

## What Monitor is

A standalone EVE Online infrastructure platform. You sign in with your EVE character (via EVE SSO)
and Monitor shows you your own data, pulled directly from CCP's ESI API:

**Assets · Ships · Inventory · Industry · Wallet · Market orders & history · Contracts · Skills ·
Blueprints · Clones · Planetary Industry · Mining** (with ore and refined ISK valuation)

Your data refreshes when you log in and on a schedule after that. You control which scopes you grant,
per character, and you can withdraw them.

It depends on no other auth platform, and it never reads another system's database.

**Current focus is pilot-facing views** — what *you* can see about *your* characters. Corp-facing
views come later.

## What Monitor reads, and what it does not

- **Only what you authorize.** Monitor asks for ESI scopes and cannot see anything you have not
  granted. The account page shows exactly which scopes each of your characters has given.
- **Location tracking and write scopes are excluded outright** — Monitor never asks for the ability
  to see where you are, or to change anything in-game on your behalf.
- Corp data needs an in-game **role**. A pilot with no roles grants nothing corp-side, and Monitor
  asks them for nothing corp-side.

## Filing a good issue

Please include:

- **What you did** — the page, and what you clicked.
- **What you expected**, and **what happened instead**.
- **Which character/page** it affected (see the opsec note below before naming anything).
- A **screenshot**, if it is a display problem — enormously helpful.
- Roughly **when** it happened, if the data looked stale or wrong.

Feature requests and "this reads badly / I misunderstood this" reports are just as welcome as bugs.
If a page confused you, that is a bug in the page.

## 🔒 Before you post — this repository is PUBLIC

Anyone can read what you write here, including people who are not in your alliance.

**Do not post:**

- **Structure names or locations** — citadels, refineries, POCOs, your PI setup.
- **Jump routes, staging systems, or where your stuff is.**
- **Asset values, wallet balances, or industry plans** you would not announce in local.
- **Tokens, refresh tokens, API keys, or anything from a URL** after you sign in.
- Anything about **another player** that they have not made public themselves.

**Redact freely.** "Ships in my staging system" is a perfectly good bug report. "Ships in <system>"
is a better one. If the detail does not change the bug, leave it out — and if you are not sure
whether a detail matters, post without it and we will ask.

**Screenshots leak.** Crop or blur item names, structure names, ISK figures, and character names in
the corner of the window before uploading. It is very easy to forget the sidebar.

If you have already posted something you should not have, say so in a comment — the issue can be
edited or deleted.

## What this repository is not

- **Not the code.** Monitor's source is not here and is not linked from here.
- **Not support for EVE itself.** If you cannot log in to EVE, or ESI is down, that is CCP's side.
- **Not a place for account problems.** Anything involving your tokens or your login belongs on
  **[Discord](https://discord.gg/rybEwArwch)**, not in a public issue.
