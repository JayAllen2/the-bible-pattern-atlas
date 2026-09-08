# The Bible Pattern Atlas

A single-file reference work tracing recurring literary, theological, structural and
typological patterns across the 66 books of the King James Version.

Open `bible_pattern_atlas_redesigned.html` in any modern browser. No build step, no
server, no network access required — everything, including the Scripture text, is
embedded in the file.

## What's inside

| | |
|---|---|
| Patterns | 209, in twelve categories |
| Book profiles | 66 |
| Section verdicts | 10 |
| Pattern chains | 8 |
| Analytical prose | ~279,000 words |
| KJV verses embedded | 10,104 |

## How it works

Everything is client-side. Three `<script>` blocks: the Atlas data, the KJV text,
and the application. Routing is hash-based (`#/pattern/A01`), so the file works
equally well from `file://` or from a static host.

**Confidence levels.** Every pattern, and most individual claims within a pattern,
carries one of four ratings — Confirmed, Very Strong, Possible, Speculative —
describing the strength of the *textual connection*, not the importance of the
truth involved. The Method page sets out the tests in full.

**Scripture is readable in place.** Every reference is a button; clicking opens the
KJV text of exactly that range. Roughly 6,000 of those references sit inside the
prose itself, so the argument and the text it argues from are one click apart.

**Guided paths.** Eleven ordered walks — three short introductory routes plus the
Atlas's own eight chains — for readers who arrive without a specific question.

**Focus mode** (the ⊙ control) strips the page to the argument and one next action,
cutting visible interactive targets roughly in half.

## Provenance of the Scripture text

The KJV text was extracted from a bundled KJV PDF and validated against the Atlas's
own 1,361 independently checked quotations:

- **92.7%** exact match
- **6.5%** superset (the Atlas abridges some quotations with an ellipsis)
- **0** references with no text found
- 31,102 verses parsed — the KJV's true verse count — across 1,189 chapters,
  with no gaps in verse numbering

Only verses actually present in the source are ever displayed. Where a cited
passage has no text available, the reader is told so rather than shown generated
text. Words in `[brackets]` were supplied by the translators and are italicised in
printed editions.

## Data corrections applied at load

- Book 22 was keyed `"Songs"`, which is not the title of any book of the canon;
  normalised to `Song of Solomon` (the KJV title) across every lookup, filter and URL.
- Quote references in the Major Prophets entries used abbreviations (`Isa`, `Jer`,
  `Ezek`) while the other ~1,346 spelled the book out; expanded for consistency.
- Fulfillment types were stored lower-case but declared capitalised in the
  methodology; normalised.

## A note on the confidence hedging

Where a claim is rated *Possible* or *Speculative*, the relationship verb shown in
the correspondence diagram is hedged ("may fulfil" rather than "fulfills"). The
category of a claim and the confidence in it are separate questions, and a
Speculative typological reading is a proposal rather than a fulfilment.

## Licence

The analytical content is the author's. The King James Version is in the public
domain in the United States; in the United Kingdom it remains under perpetual Crown
copyright, administered by Cambridge University Press, which is worth knowing if you
intend to redistribute the embedded text from within the UK.
