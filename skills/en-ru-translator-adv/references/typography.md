# Russian Typography

Apply these conventions unless the user, publisher, product style guide, or file format specifies
another standard. Preserve functional source formatting and never change code to satisfy prose
typography.

## Contents

- [Quotation marks](#quotation-marks)
- [Dashes and hyphens](#dashes-and-hyphens)
- [Lists](#lists)
- [Numbers, uncertainty, and units](#numbers-uncertainty-and-units)
- [Dates](#dates)
- [Abbreviations and spaces](#abbreviations-and-spaces)
- [Mixed-language text](#mixed-language-text)
- [The letter «ё»](#the-letter-ё)

## Quotation marks

Use Russian guillemets for primary quotations and German quotation marks for nested quotations:

- `«Основная цитата»`;
- `«Он сказал: „Это важно“»`.

Use the same marks around an English phrase quoted in Russian prose: `Система вернула сообщение
«Access denied»`. Keep straight quotes inside code and wherever syntax requires them.

## Dashes and hyphens

- Hyphen `-`: compound words and particles—`кто-то`, `из-за`.
- En dash `–`: closed ranges—`10–15 минут`, `2024–2026 годы`.
- Em dash `—`: Russian sentence punctuation and definitions—`Codex — продукт OpenAI`.

Do not replace Unicode dashes with `--`. Do not convert a minus sign, command flag, file name, or
identifier into a typographic dash.

## Lists

Keep grammar and punctuation consistent within one list. Choose the system according to the
document type rather than enforcing book punctuation everywhere.

### Complete sentences

Start with a capital letter and normally end every item with a period:

```markdown
- Навык загружается автоматически.
- Codex следует инструкциям из `SKILL.md`.
```

### Fragments continuing a lead-in

In formal or publication-style prose, start with lowercase and use semicolons, ending the last item
with a period:

```markdown
Для установки нужны:
- архив навыка;
- доступ к рабочей папке;
- средство проверки YAML.
```

### Web documentation and UI

Short labels, navigation items, feature lists, menus, checklists, cards, and UI strings may omit
terminal punctuation. Preserve the product's established pattern:

```markdown
- Documentation
- API reference
- Examples
```

Do not mix sentences and fragments accidentally. Punctuation consistency does not require adding
periods to interface labels.

### Numbered procedures

Use numbered items for sequential steps. Prefer complete commands with periods in prose
documentation. Preserve concise no-period steps when that is the established UI or house style.

## Numbers, uncertainty, and units

Typography must not change numerical meaning.

- Preserve bounds: `more than 100` → «более 100», not «100».
- Preserve approximation: `about five` → «около пяти», not «5».
- Preserve limits: `at least 3` → «не менее 3»; `up to 10` → «до 10».
- Use a comma as the decimal separator in Russian prose: `3,14`.
- Separate thousands with non-breaking spaces where the output format permits: `1 000 000`.
- Put a non-breaking space between a number and most units: `50 %`, `100 кг`, `25 °C`.
- Use ordinal endings where needed: `1-й`, `2-я`, `5-го`.

Do not alter number formatting inside code, data, identifiers, commands, or locale-sensitive input.

## Dates

Use `15 января 2026 года` or `15.01.2026` in Russian prose. Do not preserve an ambiguous numeric
date blindly: resolve it from source locale or flag the ambiguity. Keep ISO dates where required by
an API, file format, table schema, or user instruction.

## Abbreviations and spaces

Use conventional forms such as `т. е.`, `т. д.`, `и др.`, `№ 5`, and `§ 3`. Apply non-breaking
spaces only when the output format supports them and they will not break code, searchability, or
downstream processing.

## Mixed-language text

- Keep product names, identifiers, code, commands, paths, and official labels unchanged.
- Use Russian punctuation around embedded English prose when the surrounding sentence is Russian.
- Do not change capitalization that has functional or branding significance.
- Never mix Cyrillic and Latin lookalike characters in one word or identifier.

## The letter «ё»

Use «ё» consistently as this skill's editorial house style: «ещё», «всё», «её», «приём». This is
a deliberate policy for this skill, not a claim that every Russian publisher follows the same
standard. Follow an explicit customer or publication style guide if it requires selective use of
«ё».
