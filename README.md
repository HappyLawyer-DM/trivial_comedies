# A Trivial Comedy for Serious People

*Eine triviale Komödie für ernsthafte Leute — with apologies to Oscar Wilde.*

A small library of browser games about the legal profession, played with twenty-sided dice.
One arbitration, told three times over — from counsel's lectern, from the expert's chair, and
from the war room three floors below. One law firm, from the partners' floor down to the
secretariat that actually runs it. One in-house legal department at quarter's end.

No account. No install. No mercy from the printer.

**Play here:** `https://<your-name>.github.io/<repo-name>/` *(update after publishing)*

---

## The Library

| Game | Setting | Language |
|---|---|---|
| **Hearing Week** | *Dragonhoard Ventures S.à r.l. v. The Kingdom of Adverse Inference*, Vol. I — one arbitration hearing, three heads on the tribunal | EN |
| **The Expert** | The same case, Vol. II — the quantum expert's road to cross-examination, survived by giving exact change | EN |
| **The Paralegal** | The same case, Vol. III — the war room, floor −3 of the hearing; lawyers win arguments, the record wins cases | EN |
| **Equity** | Grimmwald & Finch LLP — a partners' week: a client worth keeping, a resignation worth hearing out, and the question nobody bills | EN |
| **Associate Week** | Wyrm & Grimoire LLP — an entry-level dungeon in five days; the target is 50.0, the die shows 1 | EN |
| **Fristsache** | Grimmwald & Finch, Standort Frankfurt — eine Woche im Sekretariat: rosa Zettel, ein sterbender Drucker, eine Mitternachtsfrist | DE |
| **Quarter's End** | Grevenhart Industries SE — in-house at quarter's end; trust compounds into lead time, and calm is a strategy | EN |

Each game: pick a class, keep three status bars alive, roll a d20 against the day.
Every ending is a warm one — even running out of energy just means somebody catches you.
That is not a bug. That is the thesis.

### Unlisted companion pieces

The repository may also contain a few volumes that are not on the shelf — companion pieces
for other professions, gifted privately and reachable only by direct link: *Rounds* (a hospital
week, EN), *Night Shift* (a fantasy infirmary, EN), *Nachtdienst* (eine Nacht als Dienstarzt
in einem deutschen Krankenhaus, DE) and the original guild edition of *Equity*. If you found
one of these, someone wanted you to.

---

## How it works

- **Single-file games.** Each game is one self-contained HTML file: markup, styles, engine,
  scenes and cover painting (Base64-embedded) in a single document. No frameworks, no build
  step, no external requests, no cookies, no tracking, no server logic.
- **The engine** is ~200 lines of vanilla JavaScript per game: scene graph, class bonuses,
  d20 checks against difficulty classes, three status meters, flag-based endings.
- **`index.html`** is the landing page ("the shelf"). It is fully static and works even in
  viewers without JavaScript.
- **Note for local viewing on phones:** file previews (e.g. tapping an attachment on iOS)
  do not execute JavaScript — you will only see the letterhead and a red notice. Open the
  games via the hosted link, or in a desktop browser.
- **Testing:** every game has been played end-to-end by an automated harness (jsdom) across
  random, forced-success and forced-failure dice — and, more importantly, by a real lawyer
  who kept finding the one header the search had missed.

## Hosting your own copy

1. Put all HTML files in one folder (or fork this repository).
2. On GitHub: **Settings → Pages → Deploy from branch → main**.
3. Two minutes later the shelf is live at `https://<your-name>.github.io/<repo-name>/`.

Any static host works the same way — the files have no requirements at all.

---

## The fine print

- **Everything is fictional.** All firms, companies, hospitals, cases, clients, patients,
  deadlines and colleagues are invented; any resemblance to real institutions or persons is
  unintended. The games contain jokes, not legal or medical advice. If a game and your
  professional judgment disagree, your professional judgment wins. It always should.
- **Made with AI assistance.** The games were written in long conversation with Claude,
  Anthropic's AI assistant — co-author, tireless playtester, patient re-collator of bundles —
  and the cover paintings were AI-generated. That gives the library a second, quieter joke:
  it is also a portrait of what an AI, raised on the profession's collective writing, imagines
  the law to feel like — the hearing weeks and the partners' retreats, the billable targets
  and the pink message slips, the quarter's end on the fourteenth floor; the war stories,
  the understatement, the reverence for the record, the pastries. If practitioners recognise themselves in these rooms, the credit
  belongs to everyone who ever wrote the war stories down. Concept, judgment, playtesting
  and the stubborn insistence on professional realism: human, throughout.
- **The subtitle** is borrowed from Oscar Wilde's *The Importance of Being Earnest*
  ("A Trivial Comedy for Serious People"), which is in the public domain. The apology stands.
- **Rights:** © 2026, all rights reserved. *(Placeholder — choose your own license before
  publishing; a permissive one like CC BY-NC 4.0 would suit a gift library, but that is a
  decision, not a default.)*

---

*The dice do not bill by the hour.*
