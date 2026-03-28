# Theology Claude Plugin

Version: 2026.3.28.1

A standalone Claude plugin for exegetical theology research. AI serves as a research assistant — treat output like a calculator: always verify claims, cross-reference sources, and probe answers critically.

## Skills

This plugin provides seven slash-command skills for Biblical exegesis:

| Skill | Command | Purpose |
|-------|---------|---------|
| Historian | `/historian` | Historical and cultural background |
| Linguist | `/linguist` | Hebrew, Greek, and Aramaic linguistic analysis |
| Author | `/author` | Literary features and structure |
| Theologian | `/theologian` | Theological themes, doctrines, and covenantal-canonical analysis |
| Disciple | `/disciple` | Hermeneutical methods and canonical themes |
| Shepherd | `/shepherd` | Practical modern application |
| Research | `/research` | Full exegetical analysis (orchestrates all six above) |

## Usage

### Individual Skills

Invoke any skill with a Bible passage reference:

```
/historian Genesis 1:1-25
/linguist Ephesians 2:8-10
/author Psalm 23
```

### Complete Analysis

Use `/research` for a full six-perspective exegetical analysis:

```
/research HAG 02:20-23
/research Genesis 1:1-25
```

This orchestrates all six analysis skills in parallel, compiles the output, and writes the file.

## Output

Analyses are written to: `content/<BOOK_CODE>/<CHAPTER>/<BOOK_CODE>_<CHAPTER>_<VERSES>.md`

Example: `HAG 02:20-23` → `content/HAG/02/HAG_02_20-23.md`

**Book codes** (3-letter uppercase):
GEN EXO LEV NUM DEU JOS JDG RUT 1SA 2SA 1KI 2KI 1CH 2CH EZR NEH EST JOB PSA PRO ECC SNG ISA JER LAM EZK DAN HOS JOE AMO OBA JON MIC NAH HAB ZEP HAG ZEC MAL MAT MRK LUK JHN ACT ROM 1CO 2CO GAL EPH PHP COL 1TH 2TH 1TI 2TI TIT PHM HEB JAS 1PE 2PE 1JN 2JN 3JN JDE REV

## Formatting Conventions

- **Hebrew/Greek/Aramaic terms**: `**term** (Hebrew: script, *transliteration*)`
  Example: **chotam** (Hebrew: חוֹתָם, *ḥôṯām*)
- **Biblical citations**: Book Chapter:Verses (e.g., Genesis 41:42)
- **Verse references within passage**: (v.1), (vv.1-5)
- **Strong's numbers**: H1234 or G5678 where relevant
- **Section separators**: `---` between each `## ` section
- **Subsections**: `### ` headings within each `## ` section
- **Tables**: markdown tables for comparisons, timelines, vocabulary, semantic ranges
- **Structural diagrams**: ASCII art for chiastic patterns, literary structures
- **Tone**: scholar addressing an amateur audience; confessional/evangelical, no particular tradition
