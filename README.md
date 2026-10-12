# A Trivial Comedy for Serious People

*Eine triviale Komödie für ernsthafte Leute — with apologies to Oscar Wilde.*

A small library of browser games about the legal profession, played with twenty-sided dice.
A loving tribute to tabletop games of my past and hours spent at a kitchen table rolling dice.
One arbitration, told from the lectern, the tribunal, the expert's chair and the war room three
floors below. Two law firms, from the partners' floor down to the secretariat that actually runs
them. A fantasy firm that declines no client on grounds of alignment. And the journeys in between.

No account. No install. No mercy from the printer.

**Play here:** https://happylawyer-dm.github.io/trivial_comedies/

---

## The Library

### Disputes & Procedure

| Game | File | Setting | Language |
|---|---|---|---|
| **Hearing Week** | `hearing-week-merged-tested.html` | *Dragonhoard Ventures S.à r.l. v. The Kingdom of Adverse Inference* — five days of hearing, from openings to closings, and three heads on the tribunal | EN |
| **Arbitrator Week** | `arbitrator-week-new-standard.html` | The same case from the other side of the table — as chair or co-arbitrator | EN |
| **The Expert** | `the-expert.html` | The same case, from the witness chair — the quantum expert's road to cross-examination, survived by giving exact change | EN |
| **The Paralegal** | `the-paralegal.html` | The same case, from the war room on floor −3 — lawyers win arguments; the record wins cases | EN |

### The Law Firm

| Game | File | Setting | Language |
|---|---|---|---|
| **The Associate** | `associate.html` | Grimmwald & Finch — four departments, one career | EN |
| **Der Associate** | `Associate_DE.html` | Grimmwald & Finch, Frankfurt — die deutsche Ausgabe: vier Dezernate, eine Karriere | DE |
| **Partner Week** | `partner-week.html` | Grimmwald & Finch — a partner's week: a client worth keeping, a resignation worth hearing out, and the question nobody bills *(formerly* Equity*)* | EN |
| **Associate Week** | `associate-week.html` | Wyrm & Grimoire LLP — *The Importance of Being Billable*: a first week, a target of sixty hours, and a Partners' Lounge that opens for no one. Almost. | EN |
| **Monster Files** | `Monster-Files-Case-Library.html` | Wyrm & Grimoire LLP — the fantasy firm. Six case volumes and one career, carried from case to case in a personnel file (see below) | EN |
| **Fristsache** | `fristsache.html` | Grimmwald & Finch, Standort Frankfurt — eine Woche im Sekretariat: rosa Zettel, ein sterbender Drucker, eine Mitternachtsfrist | DE |

### On the Road & Beyond

| Game | File | Setting | Language |
|---|---|---|---|
| **Travel Week** | `travel-week-optimized.html` | *Equity, continued* — three cities, one jet lag, and the road to Friday evening | EN |
| **Conference Week** | `conference-week-illustrated.html` | An arbitration conference in an unnamed host city — networking is an endurance sport | EN |

Each game: pick a class or a role, keep your status bars alive, roll a d20 against the day.

---

## Monster Files — the Case Library

*Monster Files* is a series rather than a single game: six cases from one career at Wyrm & Grimoire LLP,
the only firm in the Realm that declines no client on grounds of alignment. What matters is
solvency, a retainer and a cave address capable of service.

| Volume | Title | The matter |
|---|---|---|
| I | **The Dragon's Brief** | Ignivar's three missing chests, 340 gnomes with 2,380 names, a dead witness and the firm's first conflict of interest |
| II | **The Wizard Who Cried Sheep** | Forty-seven directors become sixty-three sheep; the insurer invokes divinity |
| III | **The Mithril Standard** | A sinking mine, a floating royal licence and a mountain claiming royalties on its own personality |
| IV | **Goblins v. Everybody** | Four hundred goblins, seven names each, and a representative who may be three people in one coat |
| V | **The Devil in the Definitions** | A devil's contract, a missing definition of eternity and a soul with interests of its own |
| VI | **Annual General Resurrection** | A company three hundred years in liquidation, undead shareholders, living proxies — and, on Saturday evening, the promotion round |

- **The personnel file.** Each volume ends with a personnel file number. The Case Library keeps it
  and hands it to the next volume: class, level, technique, standing, evidence and the decisions
  that will come back to haunt you. Conflicts are cleared between volumes; consequences are not.
- **Callbacks.** What you did in one week turns up in the next — as a line in the scene and as a
  bonus or penalty on the die.
- **Temptations.** Most scenes offer one option that is convenient, clever or what the partner
  wants. It pays at once. It costs later, in the same week.
- **The finale.** Volume VI ends with the promotion round: salaried partner (equity follows
  when the dragon pays), counsel, the rival firm with the axe on its notepaper — or adjourned
  to a date to be fixed.
- **Selected files, not six weeks.** Nobody makes partner in six weeks. Each volume is one week
  worth telling; between them lie years of leases, data rooms and waiting for other people’s
  comments, and each volume opens by saying so.
- Every volume can also be played on its own, without a file.

---

## How it works

- **Single-file games.** Each game is one self-contained HTML file: markup, styles, engine,
  scenes and cover painting (Base64-embedded) in a single document. *Monster Files* bundles its
  six volumes and the Case Library shelf into one file. No frameworks, no build step, no
  external requests, no cookies, no tracking, no server logic.
- **The engine** is a few hundred lines of vanilla JavaScript per game: scene graph, class
  bonuses, d20 checks against difficulty classes, status meters, flag-based endings and
  callbacks.
- **The die** flies across the screen and lands with the sound of a real d20 — a sound effect
  from [Pixabay](https://pixabay.com/sound-effects/search/d20/), used under the Pixabay Content
  License. With animations switched off in the operating system, the die stays put but the
  sound still plays.
- **Saving.** Most games keep nothing. *Monster Files* stores the current personnel file number
  in your browser's local storage, so that the next volume can pick it up. It never leaves
  your device; copy the number if you want to continue elsewhere.
- **`index.html`** is the landing page ("the shelf"). It is fully static and works even in
  viewers without JavaScript.
- **Note for local viewing on phones:** file previews (e.g. tapping an attachment on iOS)
  do not execute JavaScript — you will only see the letterhead and a red notice. Open the
  games via the hosted link, or in a desktop browser.
- **Testing:** every game has been played end-to-end by an automated harness (jsdom and a
  headless browser) across random, forced-success and forced-failure dice — and, more
  importantly, by a real lawyer who kept finding the one header the search had missed.

## Hosting your own copy

1. Put all HTML files in one folder (or fork this repository).
2. On GitHub: **Settings → Pages → Deploy from branch → main**.
3. Two minutes later the shelf is live at `https://<your-name>.github.io/<repo-name>/`.

Any static host works the same way — the files have no requirements at all.

---

## The fine print

- **Everything is fictional.** All firms, companies, cases, clients, deadlines, dragons and
  colleagues are invented; any resemblance to real institutions or persons is unintended.
  The games contain jokes, not legal advice. If a game and your professional judgment
  disagree, your professional judgment wins. It always should.
- **Made with AI assistance.** The games were written in long conversation with Claude,
  Anthropic's AI assistant — co-author, tireless playtester, patient re-collator of bundles —
  and the cover paintings were AI-generated. That gives the library a second, quieter joke:
  it is also a portrait of what an AI, raised on the profession's collective writing, imagines
  the law to feel like — the hearing weeks and the partners' retreats, the billable targets
  and the pink message slips, the journeys between meetings and airports; the war stories,
  the understatement, the reverence for the record, the pastries. A portrait, though, is not
  a photograph: some hardships in these games are exaggerated, others are satire outright,
  and the all-nighters arrive at a frequency no real firm would recognise. If practitioners
  recognise themselves in these rooms anyway, the credit belongs to everyone who ever wrote
  the war stories down. Concept, judgment, playtesting and the stubborn insistence on
  professional realism: human, throughout.
- **The subtitle** is borrowed from Oscar Wilde's *The Importance of Being Earnest*
  ("A Trivial Comedy for Serious People"), which is in the public domain. The apology stands.
- **Rights:** As an AI work, I keep no rights in it and no right asserted. The repository is
  released under CC0 1.0 Universal (see `LICENSE`). The one exception is the d20 sound effect,
  which stays under the [Pixabay Content License](https://pixabay.com/service/license-summary/):
  it is part of the games, but it may not be extracted and redistributed on its own.
- **Contact:** see the colophon on the shelf (`index.html`).

---

*The dice do not bill by the hour.*
