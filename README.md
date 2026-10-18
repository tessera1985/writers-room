# Writers' Room

Claude skills for screenwriters. They give notes on your pages. They never write the script for you.

*By Craig Henry*

## Why this exists

I don't believe AI, AGI or SI will ever be able to replace the creativity that comes from a human being. Our stories, our experiences, our trauma are not something that can be prompted out of an AI whose baseline is average and leans toward the average.

But a lot of screenwriting is pattern recognition. The hero's journey, the monomyth, three acts, Save the Cat: they're all patterns. AI can analyze more pages in an hour than a human can in a month. It would be a colossal blind spot not to use something that can study some of the best writing that exists and help improve yours.

## The rule

Every skill here does one of three things: gives notes, asks questions, or does research. None of them write your scenes or your dialogue. If you ask for a draft of a fix, a skill can offer one, but only for the note you asked about.

## Skills

### scene-audit

Notes on a scene, an act or a full script, the way a sharp reader in a writers' room would give them. It checks three things:

1. **Intention and obstacle.** What does each character want right now, and what's in the way?
2. **Trust the audience.** Is something said that an image already showed? Is subtext spoken out loud? Does the scene keep going past its best ending? Are the payoffs stacked so neatly that the scene feels built instead of lived?
3. **Lost me.** Is there anywhere a first-time reader can't follow?

Every note quotes the page. It says what's working, so you know what to protect. And it doesn't invent problems: if a scene works, it says so and stops.

**Example:** [a scene and its notes](examples/funeral-reception/). The scene was written by Claude from a one-line prompt. A separate Claude session audited it with only this skill and wasn't told who wrote it. Two of the notes:

> **"signals left onto Main -- though there is no one on the road to see it."**
> Designed and narrated at once. The audience can't see "no one to see it." That clause exists to explain the symbol.

> **"He says it plainly. Not as a weapon. It would be easier if it were."**
> Narrated feeling, and this one fails the strip test. "I don't know you well enough to say" is the line the scene turns on, and it can be played as a jab. Right now only the reader is told it isn't one.

**How it was tuned:** against produced TV scripts, to make sure it doesn't nag good writing, and against blind AI-written scenes, to make sure it catches what's actually wrong.

## Install

**Claude Code**

```
/plugin marketplace add tessera1985/writers-room
/plugin install writers-room@writers-room
```

Then share pages and ask for notes, or run `/writers-room:scene-audit`.

**Claude app (claude.ai)**

Customize → Plugins → Add → Add marketplace, and paste this repo's URL.

**By hand**

Copy `skills/scene-audit/` into `~/.claude/skills/`.

## Coming

More pieces of the same method: a writer's kit that does the research before you write (facts only, never dialogue), a story bible where only the writer can lock a decision, and a handoff file so a new session picks up where the last one stopped.

## License

MIT
