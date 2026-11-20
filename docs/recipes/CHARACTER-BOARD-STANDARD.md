# THE CHARACTER BOARD — our standard (v1, set 2026-11-19 by Jon + Trinity)

Every cast character in *Harlow's Helping Paws* gets ONE board in this exact format, built from their locked cast portrait. The format is harvested from the best reference boards Jon collected (an animated-3D-style Harlow board, a photoreal Chowder board, a Cash cockatiel board — banked in `cast/board-refs/`) and rebuilt as ours. **The layout is the standard; the art is always our §5 finish** (polished dimensional storybook — never the exemplars' 3D gloss or photoreal).

## How it's built (why it stays consistent)

- The **panels are generated** off the character's locked cast portrait (identity + finish authority), one strip per section.
- **All text is typeset** in the compositor (never generated) — names, labels, traits, palette hexes and checklists are always letter-perfect.
- **Palette hexes are sampled from the character's actual portrait pixels**, never invented.
- Board file: `cast/<name>-character-board.png` (2800×2100). Panels banked in `cast/board-panels/`.

## Layout (landscape 4:3, ivory board, warm hairline panel cards)

- **Left column:** character name (display serif) · "CHARACTER SHEET" · finish tag ribbon · the locked cast portrait (hero) · trait list (paw bullets, from the recipe).
- **Head shots** (5): Front · Three Quarter · Left Profile · Right Profile · Happy.
- **Turnaround / model sheet** (4, standing, one scale): Front · Left Side · Back · Right Side.
- **Expressions** (6): Neutral · Curious · Alert · Relaxed · Happy · Content.
- **Actions / poses** (8): Sitting · Standing · Walking · Looking Up · Laying Down · Stretching · Playing · Jumping / Reaching.
- **Details** (8 tiles, right column): Eye · Nose · Chin & Muzzle · Whiskers · Paw · Fur Texture · Ear · Signature feature (Harlow: tail plume).
- **Bottom band:** Color palette (8 swatches, name + hex, sampled) · Size & proportions (side-view mini + measured list from the recipe) · Key traits to maintain (checklist = the recipe's NEVER CHANGE, distilled).
- **Footer:** Style guide line — the §5 finish in one sentence + "keep consistent with this board."

## Rules

1. A board is built **only** from a locked portrait — no board before the lock.
2. Same sections, same order, same labels for every character. Species-specific swaps allowed only inside Actions and the 8th Detail tile.
3. Any panel that drifts (markings, finish, build) fails the board — regenerate that strip, never patch a board together from mismatched takes.
4. The board + the portrait are the two attachments on every future brief for that character.

## Harlow's board (first build, 2026-11-19)

Palette sampled from the canonical portrait: Tail Chocolate `#5A1D06` · Deep Seal `#612A11` · Warm Brown `#893D16` · Caramel Body `#E58944` · Cream Fur `#FDD9A2` · White Fur `#FAE5D4` · Azure Eyes `#3CB5F0` · Pink Nose `#E77C6A`.
Supersedes the six-study sheet (`harlow-character-sheet-v1.png`, kept as a take) as the board format.

## V2 AMENDMENT (Jon, 2026-11-19 late) — single-pass generated board
Jon supplied the "Universal Dimensional Animated Storybook Character Recipe V1" (banked: board-refs/universal-dimensional-storybook-recipe-v1.md) — the master recipe behind the exemplar boards he likes. V2 boards are generated in ONE gpt-image pass (Codex lane) using that recipe's §43 master-board prompt + §44 style lock, with the character's own locked portrait attached as identity authority and the exemplar board as layout guide. Our character details (identity block, measured palette, traits) replace the recipe's placeholders — identity always wins over the generic recipe (§2 conflict rule).
- Sections per §34: script name + ribbon, paw-bullet traits, hero, head shots (5), turnaround (4 — front view may sit, as in the exemplar), expressions (8), actions (8), details (8), painted palette swatches with hexes, size & proportions with dimension arrows, key traits (11), style-guide footer.
- GATE: proof every label at 3x zoom. Palette hexes verified digit-by-digit. A typo may be fixed with a surgical typeset patch (measured geometry, condensed serif, diff confined to the word box) — art is never patched; a drifting panel = regenerate.
- Harlow v2 (2026-11-19): PASSED — all hexes correct, actions clean (no cut/extra tails), one typo ("Mediuen") typeset-fixed. Canonical: cast/harlow-character-board.png (1536×1024). The v1 composited board is retired (kept as harlow-character-board-v1-composited.png).

## TEXT-BLOCK RULE (Jon, 2026-11-19 late — supersedes the typeset-patch allowance above)
If a generated board has a text error, do NOT typeset-patch it: a patched word never matches the generated hand (Jon: the other lines look "tight like a typewriter," a patch looks drawn-on and misaligned). Instead, crop the affected text panel and have the image model regenerate THAT PANEL's text (all lines, exact spellings supplied), then composite the crop back with a feathered mask and gate the seams. Harlow v4 fixed this way: Key Traits panel regenerated — all 11 lines now uniform, "Medium" correct. Canonical updated to the v4 composite.

## FOOTER STYLE LINE (Jon, 2026-11-19)
Every FUTURE character board carries a one-line style note in the footer, beside the motto "Preserve the character first; stylize second":
"Finish: Polished dimensional storybook — rich color, grouped rounded forms, warm dimensional light."
The line goes into the board generation prompt verbatim so the model typesets it with the footer. The full style prose stays in the recipe (§5) — the board gets this one line only. Harlow's board is locked as-is and is NOT regenerated for this; the rule starts with the next character (Lois).

## DRESS LOCK + HUMAN-FACE CONTENT METHOD (Jon, 2026-11-20 — from the Lois board rounds)
- **Presentation dress is LOCKED to the decorated exemplar style** — painted title treatment, floral/watercolor accents, scene-backed panels, watercolor palette dabs (the Harlow v4 / Lois v1 dress). A clean flat typeset layout is NOT an approved presentation: Lois board v3 (2026-11-20) had its content approved but its dress rejected by Jon. Typeset text is acceptable only for small panel labels inside the decorated dress.
- **Human faces are built from governed parts, not one pass.** One-pass generation genericized Lois's face twice (v1, v2). The approved method (Lois v3 content, carried into v4): hero + detail panels are REAL CROPS of the canonical portrait/full body; head shots, expressions, turnaround and actions are generated in small batches, each governed directly by the canonical portrait; the board is assembled programmatically inside the decorated dress. One-pass remains fine for animals (Harlow's identity is fur + markings).
- **Canonical maintenance:** when a canonical portrait or full body changes, the board's hero + detail crops are re-cropped from the current canonicals in the same pass. (2026-11-20: Lois's canonicals were background-warmed to the golden family tone — pale originals banked as `lois-cast-*-PALE-ORIGINAL.png` — and board v4's hero/details were re-cropped from the warmed files.)

## GRID LOCK (Jon, 2026-11-20 — the Harlow grid is THE layout for every board)
Jon's ruling after the Lois v5–v9 rounds: the layout drift between boards ends here. Harlow's approved board (cast/harlow-character-board.png) is the layout authority — every future board, human or animal, is built on this exact grid. Earlier boards composed sections freely per generation; that drift is what made Lois's board differ from Harlow's (traits mid-right, size bottom-right, boxed hero). Content flexes inside the grid (head-shot count, size treatment); POSITIONS NEVER MOVE.
- **Title + identity:** top-left — painted name, book/character-board line, HERO CHARACTER header, identity notes (paw bullets) in the left column.
- **Hero:** FREE-STANDING and large in the left-center on open garden wash — NO window box, NO border (Harlow's treatment). Zone background = plain warm ivory wash so the canonical figure blends in.
- **Head shots:** top-center window, directly right of the title block.
- **Turnaround:** directly under the head-shots window, same width.
- **Details:** right column, 8 tiles stacked, top to ~80% height.
- **Expressions:** bottom-left, two rows.
- **Actions:** center, two rows of 4, right of expressions.
- **Color palette:** bottom-left row, 8 dabs with painted names + hexes.
- **Size & proportions:** bottom-CENTER.
- **Key traits:** bottom-RIGHT.
- **Footer:** motto + finish line across the bottom.
- **Labels:** in reserved parchment bands under each window/row (the Lois fix treatment) — never touching a panel border, never painted inside a window's image area.
- **Gate addition:** every board gate now includes a LAYOUT DIFF against Harlow's board — section positions checked against this grid before content checks. A board that drifts off-grid fails regardless of content quality.

## METHOD CHANGE — ONE-PASS RECIPE IS PRIMARY (Jon, 2026-11-20)
Jon made Lois's adopted board himself in ChatGPT in ONE generation pass: four references, each with an assigned job — (1) canonical close-up = face master, (2) canonical full body = body/wardrobe master, (3) Harlow's approved board = layout template, (4) a prior board of the same character = secondary ideas only — plus a verbatim prompt spelling out every label, the grid percentages, and "full-size readable subjects instead of tiny clustered figures." Result: digit-exact palette, clean lettering, filled cells, zero seams — everything the plate-and-paste pipeline (Lois v3–v12) fought for two days. **One-pass with this recipe is now the PRIMARY board method.** Full recipe banked at cast/board-parts/LOIS-BOARD-RECIPE-JON-CHATGPT-2026-11-20.md. The governed-parts assembly method above remains the FALLBACK when a one-pass face drifts or beautifies (the Mira risk), and its gates still apply to whichever board is adopted. Adopted Lois board: cast/lois-character-board.png (Jon's one-pass, adopted 2026-11-20; the best composite, v12, stays banked as a candidate).

## THREE-PASS REFINEMENT (Jon, 2026-11-20 — from the Mira board)
The one-pass recipe extends to three passes when likeness needs tightening: (1) generate the board one-pass; (2) a LOCALIZED CORRECTION pass — re-attach board + face master, edit ONE cell only, preserve everything else (first use: a right-profile cell drawn facing the same way as the left; GATE ADDITION: always verify the two profiles face OPPOSITE directions); (3) a LIKENESS pass — re-attach board + face master and REPLACE the Front head-shot tile with the actual reference portrait as a scaled crop (crop shoulders/cap to fit; never redraw the face; keep its background), then redraw the surrounding faces toward the portrait (fuller cheeks, rounded chin, brow weight, exact nose width, smile unevenness; tone down exaggerated eyes/grins) and pull the hero's face closer too. Mira's adopted board came from this sequence (Jon in ChatGPT); full recipe: cast/board-parts-mira/MIRA-BOARD-RECIPE-JON-CHATGPT-2026-11-20.md. Known accepted deltas on that board: Cap Pink swatch prints #FDB9CB (Trinity misread it as #FDB9C8 at adoption; corrected 2026-11-20 — the lock stays #F96E6B in the recipe file), 6 short traits, blank badge tile.

**CAST BACKGROUND STANDARD (Jon, locked 2026-11-20):** solo portraits and full bodies sit on the golden warm-ivory watercolor wash ≈ RGB 252,224,184 (background only, faint grounding shadow, no scenery); boards use the same warm ivory family for their open wash and panel grounds, so a character reads identically on their portrait, their board, and any card. Never pale studio white, never a per-character hue.
