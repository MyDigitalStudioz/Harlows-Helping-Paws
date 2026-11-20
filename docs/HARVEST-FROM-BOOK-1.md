# Harvest from Book 1 — Harlow's Accidental Journey

Everything this project inherits from producing *Harlow's Accidental Journey*, so book two doesn't re-learn it. Distilled Nov 19, 2026 by Trinity. Canon lives in the book-one project; this file is the carry-over summary.

## The playbook

- **Picture-Book Production Playbook** — the master production system, at §51 as of Nov 19, 2026. Local master: `~/workspace/goals/harlow-s-big-adventure-book-production/files/PICTURE-BOOK-PRODUCTION-PLAYBOOK.md` (Drive copy is the same file, md5-matched). Sections 1–51 cover the full pipeline from recipes to Lulu proofs. Book two follows it; new lessons append to it (nightly playbook cron keeps it current).

## Print (Lulu) — proven specs from book one

- **Format:** Square 8.5×8.5, Premium Color, hardcover + paperback.
- **Cover finish:** Matte — locked for both formats (2026-11-04).
- **No ISBN** on book one.
- **Cover-start rule (locked 2026-11-04):** design covers on Lulu's real geometry from day one — casewrap face window 8.75×9 + 0.625 wrap, canvas 19×10.25, spine estimated and stamped as such. When the template returns, only the spine band moves; faces shift Δ/2; art is never rescaled or extended. Spec: book-one `files/COVER-START-SPEC-2026-11-04.md`.
- **Print-vs-file lesson (Nov 19, 2026, from Lois's hardcover proof):** casewrap fore-edge eats ~0.16" — a 0.25" file margin printed at ~0.09". Rule of thumb: give the fore-edge ≥3/8" file margin to hold 1/4" in print. Lois's verdict on book one's proof: "fantastic," "perfect," colors vibrant, nothing lopped off. Record: book-one `files/COVER-PRINT-VS-FILE-2026-11-19.md`.

## Art system — the book-one hand

- **Canon source:** the Drive **Character Recipes** set (byte-identical verified) is the canonical cast source. Briefs attach the approved portrait + paste NEVER CHANGE lines verbatim; never brief from a name, a paraphrase, or memory. Where a recipe conflicts with gold art, check the book and flag it before generating.
- **Finish:** characters = polished cast finish with dimensional cartoon lighting; objects/props/vehicles = shiny "car treatment" (glossy paint, clean reflections, gleaming chrome). Portrait background = light warm ivory watercolor wash.
- **Returning cast:** Harlow, Lois, and the '65 Mustang carry over — the Mustang interior is light blue-gray ("pale silvery blue-gray"), as in book one's gold art.
- **Render rules:** govern every revision directly off the spread's approved keeper; compare at whole frame before delivery; patch only isolated damage; if a patch round still leaves errors, regenerate the element new.
- **Hi-res rule:** deliverables are 5250×2625 via real AI upscale (Topaz High Fidelity V2, face enhancement off) — never a plain resize. Soft/washy art: blend — Topaz layer at 30% over the plain upscale.
- **Gate:** every render gets Trinity's whole-frame cartoon-polish check against the keeper before Jon sees it as a pass.

## Text authority

- Book one: the PSB (Jon's Photoshop files) is sole text authority. Book two will set its own text authority at the edit phase — until then, Lois's Google Doc is the manuscript of record.

## People & comms

- **Lois's role is deliberately light** — she writes, she notes, she interjects when she wants. Everything routes through Jon.
- **One inbox:** notes to/from Lois's Muse live in ONE shared doc — "📬 SHARED INBOX — all our notes in one place" (Mom's Notes Drive folder), entries newest first.
- **Family book operation:** book one published Nov 2026 (BEST-25d FINAL). Lois confirmed her hardcover proof Nov 19 and called it fantastic and perfect.

## Book-one repo pattern (mirrored here)

- Working branch `*-vN`; `main` = published mirror (GitHub Pages serves main); frozen `*-v1` restore point once a milestone ships.
- Standing commands (book one): "Build new book Harlow" (local only), "Publish book Harlow", "Patch book Harlow", "Flipbook: <name>".
