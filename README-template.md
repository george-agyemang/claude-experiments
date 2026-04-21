# Project Name

> One-line pitch. What it does, for whom. Example: "A CLI tool that turns my meeting transcripts into action items, built with the Claude API."

**Status:** v0.1 — working prototype / in progress / shipped
**Built with:** Claude [model name], Python/JS/etc., [any other key tools]

---

## Why I built this

Two or three sentences about the actual problem. Be specific and personal — "I kept losing track of action items from my weekly 1:1s" beats "meeting productivity is important." Hiring managers can smell a fake motivation from a mile away.

## What it does

A short demo. Pick one of these, in order of preference:

- A screenshot or GIF of it running
- A terminal recording (asciinema is free and easy)
- A code block showing input → output

```
$ python summarize.py notes/2026-04-15.txt

Action items:
1. Send Q2 forecast to Priya by Friday
2. Follow up with vendor on pricing
3. Book room for offsite
```

Keep this section tight. If someone can't understand what the project does in 30 seconds, they'll close the tab.

## How it works

A high-level walkthrough in plain English. No code dumps here — save those for the actual files.

- **Input:** What it takes in (a file, a URL, an API call, user text)
- **Processing:** The core logic. If you're using Claude, mention the model, whether you're using tool use, how you're structuring the prompt, any notable design choices.
- **Output:** What it produces and where

If there's an architecture worth drawing, include a simple diagram or a bulleted flow. Don't overdo it — three boxes and an arrow is fine.

## The prompts

This section is specific to LLM projects and is often the most important part. Either include the key prompts inline here or link to the file where they live. Prompt iteration is real engineering work; show it.

```
System prompt:
You are a meeting assistant. Extract action items from the transcript below.
Each action item must have: (1) a specific person, (2) a specific deliverable,
(3) a deadline if mentioned. Return as JSON.
...
```

## What I tried that didn't work

**This is the section most people skip and it's the most valuable one.** It signals that you can think, not just follow tutorials.

A few honest notes:

- Initially tried X, but it failed because Y. Switched to Z.
- Considered using [approach A] but rejected it because [reason].
- Still an open question: [something you haven't solved yet].

Three or four bullets is plenty. Don't invent struggles — be real about what actually happened.

## What I learned

One short paragraph. What would you do differently if starting over? What surprised you about working with the model? This is where you demonstrate reflection, which is rarer and more valuable than technical skill.

## Running it yourself

Keep this section short and executable. If it takes more than five minutes to get running, most people won't bother.

### Requirements

- Python 3.10+ (or Node 18+, etc.)
- An Anthropic API key (get one at [console.anthropic.com](https://console.anthropic.com))

### Setup

```bash
git clone https://github.com/your-username/project-name.git
cd project-name
pip install -r requirements.txt
export ANTHROPIC_API_KEY=sk-ant-...
```

### Usage

```bash
python main.py --input path/to/file.txt
```

## Roadmap / known issues

Optional but valuable. Shows you're thinking ahead and honest about limitations.

- [ ] Handle transcripts longer than context window
- [ ] Add support for Zoom's native transcript format
- [ ] Evaluate accuracy on a held-out set of 20 real meetings

Known issues:
- Currently breaks on transcripts with more than one speaker change per line
- No retry logic for API rate limits

## About me

One or two lines, with a link. Example: "Built by [Your Name]. I'm learning LLM engineering and writing about what I build at [link]. Reach me at [email] or on [LinkedIn / X]."

---

*Built while working through Anthropic's [course name] course. Part of my [claude-experiments](https://github.com/your-username/claude-experiments) portfolio.*
