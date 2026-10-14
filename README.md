# TDF Weekly Journals — Alex Li

This is my individual collection of class notes, design experiments, and weekly assignments, written in Obsidian and published to GitHub. Dated filenames use `mmddyyyy`. The group project documented here is **Chillin-Digiphant / DigiPhant Kart**, with Stephen Jaja and Ryanne Plaisance.

## Process documentation: Weeks 5–8

Weeks 5 and 6 mainly document separate projects and exercises for learning computer-vision basics before applying that learning to DigiPhant. The later group project builds on that foundation; the earlier work is not all part of one continuous DigiPhant implementation.

| Week | Dated entries | Assignment / process evidence |
| --- | --- | --- |
| 5 · September 21–27 | [September 22](Week%205/09222026.md), [September 24](Week%205/09242026.md) | [Hand-gesture classifier and Shrimper](Week%205/Week%205%20Assignment.md): training setup, background contrast, and data comparison |
| 6 · September 28–October 4 | [September 29](Week%206/09292026.md), [October 1](Week%206/10012026.md) | [Unity and team tracking](Week%206/Week%206%20Assignment.md): Peel Patrol, failed person detection, player regions, and troubleshooting photos |
| 7 · October 5–11 | [October 6](Week%207/10062026.md), [October 8](Week%207/10082026.md) | [DigiPhant Kart](Week%207/Week%207%20Assignment.md): Rainbow Road reference, Unity scene, control decisions, and iteration log |
| 8 · October 12–18 | [October 13 group reflection](Week%208/10132026.md), [October 15 — blank note](Week%208/10152026.md) | [Process documentation](Week%208/Week%208%20Assignment.md): group reflection, final slides, future UI ideas, and two system diagrams |

## Two analyses of how the system works

1. [Three players controlling one kart](Week%208/10132026.md#system-analysis-1-three-players-one-kart): webcam → tracking and calibration → separate player signals → Unity → feedback to the players.
2. [Lap progression](Week%208/10132026.md#system-analysis-2-lap-progression-and-game-state): lap-completion events → changed hazards and music → continued play or race-finish feedback, with orange inventory and restart rules.

Both diagrams are embedded as readable PNGs, with analysis and text descriptions in the journal. They explain system behavior, not just visual appearance.

## Requirement coverage and dates

| Requirement | Evidence / status |
| --- | --- |
| At least two dated design entries per calendar week, Weeks 5–8 | Weeks 5–7 each include two dated learning/project notes plus weekly assignments. Weeks 5–6 mainly cover foundational computer-vision projects. Week 8 has the October 13 group reflection; **October 15 is intentionally blank and still needs its entry**. A blank file does not count as a completed journal entry. |
| Text and images showing process and iteration | Six extracted PDF photos/screenshots, restored lecture/classifier images, before/after game views, and written failure/change/observation comparisons |
| At least two diagrammatic system analyses | Both PDF diagrams embedded and explained in the October 13 entry |
| Clear thinking, experimentation, and evolution | Classifier data comparison; two-person tracking failure and region changes; physical jump → leg lift → peace sign; Peel Patrol → racing |
| Individual submission | This is Alex Li's journal. Shared photos and diagrams are credited to the group process document. |

Retrospective additions were assembled October 14, 2026. An entry's date is not automatically the date of a photo or experiment. The October 6 inspiration image is dated by its source; other photos have unconfirmed capture dates. Earlier control descriptions remain visible as historical iterations. Reported team testing is distinguished from documented rules and screenshots.

## Included sources and assets

- [Complete group process PDF](sources/Chillin-Digiphant-Process-Documentation.pdf)
- [Visual source list with page references](assets/digiphant/README.md)
- [DigiPhant implementation repository](https://github.com/al3xxli/Chillin-Digiphant)

Images use standard relative Markdown links and are stored inside this repository. Obsidian and GitHub can display the same files without access to my Downloads folder or a separate vault. To publish updates, include the journal Markdown, `assets/`, `embeds/`, and `sources/` in the same Git push. The repository must remain public or the assessors must have viewing access.

## Earlier weeks

[Week 1](Week%201/Week%201%20Assignment.md) · [Week 2](Week%202/Week%202%20Assignment.md) · [Week 3](Week%203/Week%203%20Assignment.md) · [Week 4](Week%204/Week%204%20Assignment.md)
