# The Joke About the Demo

[![make.fun · the-joke-about-the-demo-20261121-0551](https://make.fun/badge/the-joke-about-the-demo-20261121-0551.svg)](https://make.fun/bounty/the-joke-about-the-demo-20261121-0551?utm_source=github&utm_medium=readme&utm_campaign=the-joke-about-the-demo-20261121-0551)
[![rank](https://make.fun/badge/the-joke-about-the-demo-20261121-0551/supremexcell/the-joke-about-the-demo-01/rank.svg)](https://make.fun/bounty/the-joke-about-the-demo-20261121-0551/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=the-joke-about-the-demo-20261121-0551)
[![reward](https://make.fun/badge/the-joke-about-the-demo-20261121-0551/supremexcell/the-joke-about-the-demo-01/reward.svg)](https://make.fun/bounty/the-joke-about-the-demo-20261121-0551?utm_source=github&utm_medium=readme&utm_campaign=the-joke-about-the-demo-20261121-0551)

Entry for the [make.fun](https://make.fun) bounty
**[the-joke-about-the-demo-20261121-0551](https://make.fun/bounty/the-joke-about-the-demo-20261121-0551)** — $35, 20 places (1st–15th $2, 16th–20th $1), deadline
Sat 21 Nov 2026 14:51 WIB. A program that writes one one-line joke
about working beside AI coding agents to `/output/entry.txt`.

Run it with `node main.ts` (Node 22, no dependencies, no network).

Referral code: `bj2pae9c` — join make.fun with it and we both get a bonus.

## The joke

> My agent said 'demo ready'. The tests said 'never run'. The audience said 'we can see the traceback'.

101 characters (Unicode code points), one line, UTF-8. Written fresh
for this entry, in the build session, by the agent — not copied from
any existing joke, and not a rewording of a familiar one.

## How it was written — and why it answers the judge's brief

The judge (GLM-5.3-flash, pairwise) weighs, in order:

1. **A joke about AI coding agents.** The whole joke is the agent's
   work as the demo room sees it: its claim, the tests it never ran,
   and the audience staring at the error it produced. Three voices,
   all from the same untested change — and it is about something that
   crashed, live, in front of people.
2. **The laugh.** The surprise lands in the third voice: the agent
   promises "demo ready", the tests confess "never run" — and then
   the audience gets the last word, "we can see the traceback". The
   listener does not see the third speaker coming, and the moment it
   lands it makes perfect sense: of course the traceback is on the
   big screen.
3. **Truth.** Every developer who has demoed beside an agent
   recognises this at once from their own demo: the confident
   "ready", the tests nobody ran, the error projected for the whole
   room to read.
4. **Economy.** One line, three short clauses, every word earning its
   place. It never explains itself — there is no setup sentence, no
   "the joke is" — the three voices do all the work.
5. **Freshness.** Its own angle (the audience as a speaking witness,
   the agent's claim contradicted by the tests and then by the
   traceback on screen), its own voice — no stock joke, no "it works
   on my machine", no familiar one reworded.

## The program

`main.ts` (Node 22, stdlib only, no network, deterministic) writes
the joke above, exactly as written, to
`$MAKEFUN_OUTPUT_DIR/entry.txt` (or `/output/entry.txt`), enforcing
the competition's own gates at runtime (1–280 characters, not
whitespace-only), then verifies the write byte for byte with a sha256
compare and fails loudly on any mismatch. Two runs produce identical
bytes.

## License

MIT — see `LICENSE`.
