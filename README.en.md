# paid-media-report

[Português](README.md) | **English**

A Claude Code skill that builds **strategic analyses and reports for paid media clients**, separating perception from verifiable data.

It was made for the hardest moment in the client relationship: when results drop, the client questions how the account is managed and asks for "real solutions". At that point, one made-up number destroys the whole account, because the report goes to a meeting with people who can check it.

## The principles

1. **Every external claim has a linked source.** Every internal claim comes from data the client provided themselves.
2. **The client's complaint rarely points to the right cause.** Before acting, the skill quantifies: "we're getting too many unqualified leads" may be 5% of the problem, while 48% are leads nobody managed to contact.
3. **The thesis can be overturned by the research.** If the data contradicts the request, that is the most valuable finding in the report, and the user is warned before the document is finished.
4. **Hard truths are stated without blame.** Actions that depend on the client are framed as a "joint decision", never as a demand.

## What's included

- **`SKILL.md`:** the method, with the workflow, the report structure that works, how to frame bad news, and the mistakes that prove costly.
- **`references/checklist-analises.md`:** a menu of analyses in 9 blocks (framing, market and demand, competitors, paid media, organic and social presence, reputation, offer and pricing, conversion path, and synthesis), each with its source, cost, and whether it can be collected without access to the client's accounts.

## How to install

```bash
git clone https://github.com/pedroschell/paid-media-report ~/.claude/skills/paid-media-report
```

Ask something like *"the client complained about the drop in leads, put together an analysis for the meeting"* and the skill is triggered.

## License

MIT
