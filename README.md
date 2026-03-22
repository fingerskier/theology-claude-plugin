# theology-claude-plugin

A standalone Claude plugin for exegetical theology research. Teaches Claude how to conduct rigorous, multi-perspective Biblical exegesis.

## What It Does

This plugin provides seven slash-command skills that analyze Bible passages from different scholarly perspectives:

- **`/historian`** — Historical and cultural background (authorship, dating, archaeology, geography, social context)
- **`/linguist`** — Hebrew, Greek, and Aramaic linguistic analysis (word studies, grammar, etymology, translation comparison, textual variants)
- **`/author`** — Literary analysis (genre, structure, chiasm, rhetorical devices, numerology, symbolism)
- **`/theologian`** — Theological themes and doctrines (original audience understanding, spiritual disciplines, timeless principles)
- **`/disciple`** — Hermeneutical analysis (canonical themes, wordplay, micro/macro structures, plenary authorial intent)
- **`/shepherd`** — Practical application (bridging ancient meaning to modern life, what must change, implementation guidance)
- **`/research`** — Full exegetical analysis (orchestrates all six skills in parallel and compiles a complete document)

## Installation

Clone this repository into your project or add it as a git submodule:

```bash
git clone https://github.com/fingerskier/theology-claude-plugin.git
```

The `.claude/skills/` directory contains the skill definitions that Claude Code automatically discovers.

## Usage

```
/research Genesis 1:1-25
/historian Psalm 23
/linguist Ephesians 2:8-10
```

The `/research` command runs all six analysis skills in parallel and produces a comprehensive exegetical document written to `content/<BOOK_CODE>/<CHAPTER>/`.

## Output

Each analysis follows a consistent scholarly format with:
- Hebrew/Greek/Aramaic terms with transliteration
- Strong's concordance numbers
- Markdown tables for timelines, vocabulary, translations, and comparisons
- ASCII diagrams for literary structures
- Cross-references throughout

Tone: scholar addressing an amateur audience; confessional/evangelical, no particular tradition.

## License

MIT
