# Conversation-to-Commerce

> An AI that reads purchase intent from a social comment and completes the order in a private DM — so a casual craving becomes a confirmed order **without the user ever leaving the app they're already in.**

## The problem

We discover food everywhere now — a reel, a friend's story, a thread about the best pizza in town. But to actually order it, we leave the app, open a delivery app, search the restaurant, find the dish, rebuild the order, and check out. **Intent leaks at every step.**

## The reframe

The obvious first idea — order straight from a comment via a quick form — fails the only question that matters: *if you still pick the restaurant, type your address, and pay, why wouldn't you just open the app?* It's faster.

Changing the entry point isn't the same as removing the work. So this isn't "another way to order." It **captures intent at the moment of discovery** — the one moment the delivery app is weakest, because it forces you to abandon what you're looking at to go buy it.

## How it works

```
public comment  →  AI detects intent  →  private DM  →  order rebuilt from history  →  one-tap confirm  →  live tracking
```

The order moves to a DM so address and payment stay private, and the AI does the assembly — the user's only decision is which option to tap.

## What's in this repo

| File | What it is |
| --- | --- |
| `index.html` | The interactive prototype — a single, self-contained file (no build, no dependencies) |
| `Social_Commerce_AI_Case_Study.pdf` | The full product case study: problem, reframe, architecture, constraints, roadmap |

## Run it locally

```bash
git clone https://github.com/<your-username>/conversation-to-commerce.git
cd conversation-to-commerce
open index.html      # or just double-click it
```

No install step — it runs in any modern browser.

## Built to be honest

The case study deliberately treats the two things that decide whether this is *buildable*, not just desirable, as first-class design constraints:

- **Platform messaging policy** — you can't DM a user uninvited; a public comment is what opens a compliant window.
- **Social-listening API economics** — monitoring mentions at scale gets expensive fast, which shapes who can realistically build it.

## A note on scope

This is a **click-through prototype** (HTML/CSS/JS) built to communicate the concept end to end — not a production app. The brand ("Crave"), pricing, and addresses are illustrative.
