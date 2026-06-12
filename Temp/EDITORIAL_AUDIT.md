# Editorial Audit — First Pass

Date: 2026-06-12

This file records the first safe editing pass completed after cloning the repository. Because no specific story change was requested, this pass focused on low-risk structure, Markdown hygiene, and navigation rather than changing canon or rewriting scenes.

---

## Edits completed

- Added a root [`README.md`](../README.md) so the repository has an entry point on GitHub.
- Normalized Markdown whitespace across the repo:
  - removed trailing spaces/tabs from Markdown lines;
  - ensured Markdown files end with a final newline.
- Added a missing top-level title to:
  - `Sabrina Bryna and William/Taylor Raven/taylor-raven-key-profile.md`
- Cleaned `Temp/OPEN ITEMS.md`:
  - removed a duplicate `Vacations/` open-item bullet;
  - fixed the Markdown formatting for the `Vacations/` path by using backticks.

---

## Repository snapshot

- Markdown files: 205 before this pass; 207 after adding `README.md` and this audit.
- Main reference files:
  - `Temp/TIMELINE.md`
  - `Temp/OPEN ITEMS.md`
  - `Temp/Medical Information.md`
- Largest branch: `Patti Anne and Aleksander/`, especially the Gamaliel/Klára/Prague material.

---

## Structural items to review next

These were not changed in this pass because they could affect canon, links, or file history.

### 1. Duplicate or backup files

Potential cleanup candidates:

- `Jessica Isabella and Emma/colleague-donor-arc-outline.md.bak`
- `Patti Anne and Aleksander/Gamaliel Galvin and Klárá/Simonka Káta and Holic/18 years/simonka-meets-advisor-monday-three-oclock-scene-outline 2.md`
- `Patti Anne and Aleksander/Gamaliel Galvin and Klárá/Simonka Káta and Holic/Good Girl/monday-morning-gg-comes-out-scene-outline 2.md`

Recommended next step: compare each pair, merge anything unique, then delete or archive the duplicate with an explicit note.

### 2. Unicode path normalization

Several folder names use accented characters in a decomposed Unicode form, especially the Klára/Klárka/Simonka branch. This can display normally while still causing portability issues across systems.

Recommended next step: decide whether to keep accented names in paths or rename folders/files to ASCII-only slugs, then update any internal references consistently.

### 3. Heading hierarchy

A small number of files contain multiple `# H1` headings. That can be intentional for anthology/combined files, but it makes navigation less predictable.

Recommended next step: for each combined file, decide whether repeated `#` headings should become `##` section headings or whether the file should be split.

### 4. Timeline anchors

`Temp/OPEN ITEMS.md` already identifies several timeline questions that gate downstream scenes. The highest-value continuity edits appear to be:

- Carlota Delicia's exact diagnosis/rescue/disclosure timeline.
- The Prague academy gift/trust mechanics.
- Whether vacation material intersects the Mike-death arc.
- The exact calendar around Mike's death, funeral, and the daughters' grief scenes.

### 5. Mature or traumatic arcs

Some branches include mature, medical, coercive, or traumatic material. Before doing a prose rewrite on those scenes, set explicit editorial boundaries for tone, age/timeline clarity, consent, and how much detail belongs on-page versus implied or summarized.

---

## Recommended next editing pass

If you want the repo improved without changing canon, the next best pass is:

1. Create or update a master character index.
2. Merge/delete duplicate backup files.
3. Standardize file titles and heading hierarchy.
4. Add a short synopsis at the top of each major folder's main `.md` file.
5. Convert resolved timeline decisions from scattered scene notes into `Temp/TIMELINE.md` and check off matching items in `Temp/OPEN ITEMS.md`.
