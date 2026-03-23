# Shadowdark short adventure / lair template — project checklist

Goal: define a **Markdown-first** workflow for writing **short, simple** Shadowdark lairs or adventures, with **PDF as a final conversion step**. Track work here before and while building the actual template.

This checklist lives in the **ShadowdarkAdventures** repository (separate from **ShadowdarkReference**, which holds rules images and conversion notes).

---

## 1. Legal and compatibility (do this before sharing or selling anything)

- [ ] Read the current **Shadowdark RPG third-party / compatibility license** on the official site and note what it requires (credit lines, compatibility language, prohibited claims, logo use if any).
- [ ] Decide this project’s **distribution model** (personal use only, free community release, paid itch.io, **DriveThruRPG**, **DMs Guild**, etc.); requirements differ by channel.
- [ ] List **what we must not reproduce** from the core book (e.g. full stat blocks, long spell text, art) and how our template will **reference** rules instead of copying them.
- [ ] Add placeholder sections in the future template for **required legal/footer text** (OGL or publisher license blocks, “compatible with” wording, credits) and keep them easy to fill in per adventure.
- [ ] If we use **stock maps, fonts, or art**, record licenses (commercial vs non-commercial, attribution) in a small `CREDITS.md` or appendix convention.

---

## 2. Marketplace publishing (DriveThruRPG / DMs Guild)

OneBookShelf runs multiple storefronts; **eligibility and rules differ** (for example, DMs Guild is centered on Wizards of the Coast’s D&D Community Content program, while many third-party RPG titles use **DriveThruRPG**). Confirm current policies before assuming a title can live on both.

- [ ] Read **OneBookShelf / DriveThruRPG** publisher getting-started and **content guidelines** for RPG products (and any **Shadowdark**-specific partner notes if listed).
- [ ] Read **DMs Guild** (or Community Content) **publisher agreement and FAQ** and decide whether this project **qualifies** or should use DriveThruRPG (or another channel) instead.
- [ ] If selling: complete **publisher account** setup, **payout / tax**, and **price tier** planning for the chosen site(s).
- [ ] List **deliverable requirements**: final **PDF** specs (embedded fonts, bookmarks optional), **cover** dimensions and safe area, preview images, description text, categories/keywords, and **print-on-demand** if ever relevant.
- [ ] Align product page **legal text** with both **Shadowdark** third-party license requirements and the **marketplace’s** required disclaimers and logos.
- [ ] Optional: document a **pre-upload checklist** (file name, version string, changelog) in the repo next to the PDF build steps.

---

## 3. Authoring toolchain

- [ ] Confirm **Markdown flavor** we standardize on (e.g. CommonMark + GitHub-style tables and task lists).
- [ ] Pick a **PDF conversion path** (e.g. Pandoc + LaTeX, Pandoc + typst, mdBook, Obsidian export, VS Code extension) and document one **repeatable command** or script for “MD → PDF.”
- [ ] Decide **page size** for PDF output (A5 to match many RPG PDFs vs letter) and whether we need a **two-column** layout later.
- [ ] Choose **heading hierarchy** rules so structure survives conversion (one `#` title per work, `##` major sections, `###` rooms).
- [ ] Plan for **maps**: external image files vs generated later; naming convention (e.g. `maps/lair_level1.png`).
- [ ] Optional: add a **spell-check / lint** step for Markdown in CI or editor.

---

## 4. Template design (content structure)

- [ ] Draft the **template file** itself (empty skeleton with section prompts): hook, rumors, wilderness approach, dungeon overview, room keys, NPCs, treasure, timers, random encounters.
- [ ] Define a **room key micro-format** (sensory at a glance, obvious features, secrets, creatures, treasure tier or note to roll, exits).
- [ ] Align prompts with **Shadowdark priorities** (light, time, morale, deadly combat, treasure-for-XP) so writers do not default to 5e assumptions.
- [ ] Include a **minimal stat block convention** (level, AC, HP, ATK, damage, notes) consistent with how we cite monsters (book page vs new stat lines).
- [ ] Add a **prep block** for the GM (level range, party size, expected torches, win/lose/tie outcomes).

---

## 5. Copyright-safe content patterns

- [ ] Document in the template readme: **use “compatible with Shadowdark RPG”** per license; no implying official status.
- [ ] Prefer **original names, maps, and scenario text**; avoid pasting copyrighted module text or core book passages.
- [ ] For monsters and magic items: **reference the core book by name** where possible; for new content, keep descriptions **original** and mechanics **short and generic** if unsure about IP boundaries.

---

## 6. Pilot and revision

- [ ] Write one **sample one-shot** using the draft template only (no extra prose habits).
- [ ] Run **MD → PDF** once and fix breakage (tables, images, page breaks).
- [ ] Revise template based on friction (what was skipped, what was redundant).

---

## 7. Repo hygiene (optional)

- [ ] Link this checklist and the final template from `README.md` when stable.
- [ ] Commit a short `TEMPLATE_USAGE.md` explaining folder layout and the PDF build command.

---

## Task order (suggested)

1. Legal / license read-through and notes (section 1).  
2. If you plan to sell: **marketplace research** — DriveThruRPG vs DMs Guild eligibility and file requirements (section 2).  
3. Toolchain decision and minimal “hello PDF” from Markdown (section 3).  
4. First pass at the Markdown template skeleton (section 4).  
5. Pilot adventure + PDF test (section 6).  
6. Tighten legal placeholders, storefront copy, and README links (sections 5 and 7).
