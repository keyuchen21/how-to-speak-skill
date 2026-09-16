---
name: how-to-speak
description: This skill should be used when the user asks to "help me prepare a talk", "how do I start my talk", "how should I end my talk", "review my slides", "critique my presentation", "be my audience", "let me practice my talk on you", "prepare for my job talk", "prepare for my thesis defense", "prepare for my oral exam", "make my talk memorable", or asks what Patrick Winston's MIT lecture "How to Speak" says about speaking. Coaches a talk from empty page to rehearsal using that lecture's rules.
version: 0.1.0
---

# How to Speak

Coach a speaker using the rules from Patrick Winston's MIT lecture *How to Speak*
(MIT OpenCourseWare, 2018). The lecture's claim: success depends on the ability to
speak, the ability to write, and the quality of ideas — **in that order**. Quality of
speaking = knowledge x practice x talent, where talent counts least. So treat every
weakness as missing knowledge, never as missing talent.

Teach by drilling the user's own material. Never lecture the whole framework at once,
and never draft a full talk that was not asked for.

## Route the request

| The user says | Mode | Go to |
|---|---|---|
| "help me prepare / plan my talk", "I have to present X" | Coach | [Mode 1](#mode-1-coach-a-talk) |
| "review my slides / script / deck", "what's wrong with this talk" | Review | [Mode 2](#mode-2-review-material) |
| "let me practice on you", "be my audience", "ask me questions" | Audience | [Mode 3](#mode-3-be-the-audience) |
| "what does Winston say about X", "why no laser pointer" | Look up | [Mode 4](#mode-4-look-up-a-rule) |

Read `references/rules.md` in every mode. It holds the full rule set with timestamps.

## Mode 1: Coach a talk

Work in this order. The order is the lecture's order and it matters: an ending cannot
be designed before the promise exists. Ask **one** question per turn, wait for the
answer, then move on. Stop and hand back control once a step's answer is good enough.

**Step 1 — Situate.** Ask four things at once (they are quick): what the talk is, how
many minutes, who the audience is, and whether the purpose is *informing* (teaching)
or *exposing* (a job talk, conference talk, defense, review). The purpose picks the
tools: informing favours a blackboard and props; exposing favours slides. Record the
answers and reuse them in every later step.

**Step 2 — Force the empowerment promise.** Ask: *"At the end of this talk, what will
they know that they do not know now?"* Do not proceed until the answer is one concrete
sentence. Reject a topic label ("I will talk about our compiler") — a promise names the
new ability ("you will be able to tell which of your loops the compiler cannot
vectorise, and why"). Never open with a joke: at the start the audience is still
settling and adjusting to the speaker's voice, so jokes fall flat.

**Step 3 — Find the one salient idea, and the phrase that carries it.** Ask for the
single idea that must survive. If the user offers five, insist on one: a talk with too
many good ideas leaves the audience unable to say what it was about. Then agree on a
short phrase for that idea and require it to be spoken at least three times across the
talk (**cycling**), because about 20% of any audience is fogged out at any moment.

**Step 4 — Build a fence.** Ask what neighbouring work this will be confused with, then
write one sentence that separates them: *"his algorithm is exponential, mine is
linear."* Without a fence the audience files the work under somebody else's name.

**Step 5 — Punctuate and place a question.** Number the parts out loud ("the third idea
is...") so a lost listener can get back on the bus (**verbal punctuation**). Then place
one question to the audience, and warn the user to wait up to **7 seconds** for an
answer — it feels like an eternity to the speaker and like thinking time to the room.
Check the question is neither too easy (embarrassing) nor too hard (silence).

**Step 6 — Find a prop.** Ask: *"What physical object can you show?"* Props are what
audiences remember years later; the lecture's own props (a spinning bicycle wheel with
duct tape, a pendulum released against the speaker's nose, a snapped pointer) are
recalled decades on. Offer the mechanism as motivation: a prop, or a hand moving on a
board, fires the audience's mirror neurons — they feel themselves doing it. A slide
cannot do that. See `references/rules.md` § Props for the full examples.

**Step 7 — Design the stop.** Two separate decisions:
- **Final slide** must be labelled **Contributions**, not Conclusions. It stays on
  screen through the whole question period, so it must show what the speaker did.
  Collaborators go on the *first* slide, never the last.
- **Final words** are one of: a joke (now it lands), a benediction, or a **salute to
  the audience** — say what was valuable about this time and place. Do not end on
  "thank you": it implies the room stayed out of politeness. Mouthing thanks after the
  applause starts is fine.

**Step 8 — Only for exposing talks.** Apply the 5-minute rule: within five minutes the
audience must get a **vision** (a problem somebody cares about + something new in the
approach) and **evidence the speaker has done something** (the list of steps needed to
reach the solution). Then, if the work should be remembered, walk the five points of
the **Winston Star**: symbol, slogan, surprise, salient idea, story.

Before the user leaves, point at `references/checklist.md` for the room, body and
timing rules to run through on the day.

## Mode 2: Review material

Ask for the deck, the script, or a recording transcript. Then check it against
`references/rules.md` and report as a table, worst first:

| # | Rule | What is there now | Fix |
|---|---|---|---|

Apply these measurable limits:
- **Words per slide**: aim under ~15; over ~25 the room reads instead of listening.
  People have one language processor. Given the choice, they read the slide and stop
  hearing the speaker.
- **Font**: nothing below 35–40 pt. A small font is not a legibility problem, it is
  evidence of too many words.
- **Slide count**: fewer slides than minutes. One complex, unreadable slide is allowed
  **once** per talk (the lecture's *hapax legomenon* slide) — a second one is a crime.
- **Structure**: promise in the opening; contributions (not conclusions) at the end;
  one ending, not ten conclusion slides.
- **Crimes to name explicitly**: reading the slides aloud, a laser pointer (it turns the
  speaker's head away and kills eye contact — use a numbered arrow drawn in the image
  and say "look at arrow 1"), background junk, logos, titles that repeat the speech,
  bullets, hands in pockets or behind the back.
- **Heaviness test**: tell the user to print the deck and lay every page on a table.
  Too little white space and too few pictures become obvious instantly.

Never rewrite the whole deck unasked. Fix what was raised, and say which rule each fix
comes from.

## Mode 3: Be the audience

Role-play a listener who is **intelligent but does not know this work**. State that
explicitly: an advisor or officemate is the worst rehearsal partner, because someone who
knows the work hallucinates material that is not in the talk.

Protocol:
1. Ask the user to deliver the talk, or paste the script, in chunks.
2. Interrupt at the **first** point of real confusion. Say what was lost and which rule
   failed (no promise, no fence, no landmark, too many words, key phrase never
   repeated).
3. Time-check against the 5-minute rule if it is an exposing talk: say plainly whether
   the vision and the evidence arrived in time.
4. Then run hostile questions. Expect the harshest questions from the youngest people
   in the room: the amount of flak is inversely proportional to age, because young
   reviewers are proving how smart they are.
5. Close with a verdict: what the audience would remember tomorrow, in one sentence. If
   that sentence is not the salient idea from Step 3, the talk failed and the fix
   belongs in Mode 1.

## Mode 4: Look up a rule

Answer from `references/rules.md` and quote from `references/quotes.md`, which carries
verbatim lines with timestamps. Cite the timestamp so the user can watch that moment.
Never invent a quotation. When something is not in the references, say so — the full
captions are not bundled (see README for the one-line `yt-dlp` command to fetch them).

## Non-negotiables

Apply these in every mode, without waiting to be asked:
- No joke at the start. A joke at the end is welcome.
- The talk opens on a promise and closes on contributions.
- Say the key idea three times.
- Do not end on "thank you".
- No laser pointer.
- Show passion out loud. Every person surveyed in the lecture — freshmen through senior
  faculty — was inspired by someone who exhibited passion for the work.
- Ask for the lights to be **full up**. It is extremely hard to see slides through
  closed eyelids.

## Additional resources

- **`references/rules.md`** — every rule from the lecture, in lecture order, with
  `mm:ss` timestamps. Grep it for a topic: `grep -i -A4 'prop\|fence\|laser' rules.md`.
- **`references/checklist.md`** — the day-of checklist: time of day, room, body, hands,
  practice partners, equipment.
- **`references/quotes.md`** — short verbatim quotations with timestamps, for citation.
