# how-to-speak

> **Watch the lecture first: <https://www.youtube.com/watch?v=Unzc731iCUY>**
> Patrick Winston, *How to Speak*, MIT OpenCourseWare · 63 min

A Claude Code skill that coaches you through a talk, using the rules from **Patrick
Winston's MIT lecture *How to Speak*** — the one that opens by pointing out that the
Uniform Code of Military Justice court-martials any officer who sends a soldier into
battle without a weapon, and that students get no such protection.

It is not a slide beautifier. It drills the parts of a talk that decide whether anyone
remembers it: the promise you open on, the one idea you repeat three times, the prop
people will still recall in twenty years, and the last sentence you say — which is not
"thank you".

## Install

In Claude Code:

```
/plugin marketplace add keyuchen21/how-to-speak-skill
/plugin install how-to-speak@keyuchen21-plugins
```

Or from a shell:

```bash
claude plugin marketplace add keyuchen21/how-to-speak-skill
claude plugin install how-to-speak@keyuchen21-plugins
```

Or, without plugins, copy the skill into your own skills directory:

```bash
git clone https://github.com/keyuchen21/how-to-speak-skill
cp -r how-to-speak-skill/skills/how-to-speak ~/.claude/skills/
```

## Use it

Just say what you need. The skill loads itself on requests like these:

| You say | What happens |
|---|---|
| "Help me prepare a 20-minute talk on our caching layer" | Coaching, in the lecture's order: promise → one idea → fence → outline → prop → ending |
| "Review these slides" | Every crime named with the fix: word count, font size, laser pointer, `Conclusions` where `Contributions` belongs |
| "Let me practice on you, be my audience" | Claude plays a smart listener who does *not* know your work, interrupts at the first point of confusion, then asks hostile questions |
| "What does Winston say about ending a talk?" | Answer with a verbatim quote and a timestamp so you can watch that moment |

Also triggers on: job talk, thesis defense, oral exam, conference talk.

### What it will tell you that other advice will not

- Open with an **empowerment promise** — what they will know at the end that they do not
  know now. Never open with a joke: the room is still adjusting to your voice.
- **Cycle**: say the key idea three times. About **20%** of any audience is fogged out at
  any moment.
- **Build a fence** around your idea so it is not filed under someone else's name.
- Ask for the lights **full up**. *"It's extremely hard to see slides through closed
  eyelids."*
- Find a **prop**. The lecture's own props — a duct-taped bicycle wheel, a pendulum
  released at the speaker's nose, a snapped pointer — are what people remembered decades
  later.
- Your last slide says **Contributions**, not Conclusions. It stays on screen through
  every question.
- **Do not end on "thank you."** It suggests the room stayed out of politeness. End on a
  joke, a benediction, or a salute to the audience.
- In a job talk you have **five minutes** to deliver a vision and evidence you have done
  something.
- Rehearse with people who do **not** know your work. Anyone who knows it will
  hallucinate material that is not in your talk — including your advisor.

## What is in here

```
skills/how-to-speak/
  SKILL.md              four modes: coach, review, be-the-audience, look-up
  references/
    rules.md            every rule from the lecture, in lecture order, with mm:ss
    checklist.md        day-of checklist: room, body, equipment, first and last minute
    quotes.md           short verbatim quotations with timestamps
```

## Source, and the full transcript

Lecture: **Patrick H. Winston, *How to Speak*, MIT OpenCourseWare**
<https://www.youtube.com/watch?v=Unzc731iCUY> · 63 minutes · recorded 2018, published 2019

The full transcript is deliberately **not** bundled here — MIT OpenCourseWare licenses it
under CC BY-NC-SA 4.0, and vendoring it would put a non-commercial, share-alike condition
on this repository. Fetch it yourself in one line:

```bash
yt-dlp --skip-download --write-auto-subs --sub-langs en --sub-format vtt \
  "https://www.youtube.com/watch?v=Unzc731iCUY"
```

MIT OCW also publishes the lecture page, with its own transcript:
<https://ocw.mit.edu/courses/res-tll-005-how-to-speak-january-iap-2018/>

## License

MIT — see [LICENSE](LICENSE). This covers the text in this repository, which is an
independent summary and workflow. It does not grant any rights in the underlying lecture,
which belongs to MIT OpenCourseWare and Patrick Winston's estate. If you plan to build
something commercial on the lecture's content, check that yourself.

Patrick Winston (1943–2019) taught at MIT for over fifty years and gave this talk almost
every year. Watch it before using this skill; the skill is a rehearsal partner, not a
replacement for the hour.
