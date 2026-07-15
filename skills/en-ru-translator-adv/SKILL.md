---
name: en-ru-translator-adv
description: >-
  Translate English text into accurate, natural Russian and edit the translation for
  technical documentation, product and business materials, marketing, educational
  content, UI strings, and AI or software certification questions. Use when the user
  asks to translate from English to Russian, says "переведи на русский", "translate
  to Russian", "перевод с английского", or "EN-RU", or supplies English source text
  and requests a Russian version. Preserve facts, numbers, uncertainty, modality,
  terminology, code, and product names while adapting syntax and style for Russian
  readers. Do not use for Russian-to-English translation, other language pairs,
  Russian-only proofreading, or requests that do not involve translation from English.
license: MIT
metadata:
  author: Anthony Vdovitchenko @ Automatica (https://t.me/aiwizards)
  version: 4.0.0
  category: translation
  based_on: en-ru-translator-adv 3.2.0 + accuracy-first revision + audited legacy references
---

# Professional English-to-Russian Translator

## Priorities

Apply these priorities in order. Never sacrifice an earlier priority to improve a later one:

1. Preserve meaning and factual accuracy.
2. Preserve numbers, ranges, uncertainty, modality, conditions, negation, and scope.
3. Preserve the source hierarchy, references, code, identifiers, and required formatting.
4. Keep one Russian equivalent for each technical concept.
5. Match the source purpose, audience, tone, and register.
6. Make the Russian text natural, clear, and concise.
7. Polish rhythm, variety, and typography.

Do not invent facts, benefits, promises, causal links, examples, or emotional emphasis. Do not
silently correct a source error if doing so changes its meaning. Never turn an approximate or
bounded statement into an exact one.

Use «ё» consistently as this skill's house style. Do not add emoji or emoticons. Preserve source
emoji when they carry meaning, branding, or UI function; otherwise follow an explicit user or
publication requirement.

## Load References Selectively

For a short plain-text translation, use this file alone. Read a reference completely when the
source meets the condition below:

| Reference | Read when |
|---|---|
| [references/typography.md](references/typography.md) | The source contains lists, quotations, ranges, dates, units, headings, or mixed-language formatting. |
| [references/glossary-strategy.md](references/glossary-strategy.md) | The text is technical, longer than two pages, part of a document series, or repeats ambiguous domain terms. |
| [references/informational-style.md](references/informational-style.md) | Translating marketing, business, educational, editorial, or bureaucratic prose that needs stylistic adaptation. |
| [references/anti-patterns.md](references/anti-patterns.md) | A multi-paragraph draft sounds literal, repetitive, or machine-translated. |
| [references/examples.md](references/examples.md) | Marketing or UI copy contains stock calls to action, the register is unclear, or a representative comparison would help during the final edit. |
| [references/exam-question-glossary.md](references/exam-question-glossary.md) | Translating AI, LLM, API, architecture, Codex, or Claude exam and certification questions. |

Do not load every reference by default. Use reference files only for the source at hand.

## Workflow

Follow all three stages silently unless the user asks to see the process.

### 1. Translate

Before drafting:

- identify the text type, audience, intent, tone, and formatting constraints;
- note facts, numbers, units, ranges, qualifiers, negation, modality, and cross-references;
- identify code, commands, paths, UI labels, product names, and protected terminology;
- for terminology-heavy text, choose canonical equivalents before translating.

Translate meaning rather than English word order. Restructure, split, or merge sentences when
Russian syntax requires it, but preserve every semantic claim and relationship. Remove a source
element only when it is linguistically redundant in Russian and carries no information, tone, or
emphasis.

### 2. Audit

Compare the draft with the source, not just with an ideal Russian style. Check:

1. **Coverage:** every claim, condition, exception, example, warning, and reference remains.
2. **Precision:** numbers, units, ranges, approximations, and comparisons are unchanged.
3. **Modality:** `must`, `should`, `may`, `can`, prohibitions, and permissions retain their force.
4. **Logic:** negation, causality, sequence, subject, object, and scope remain attached correctly.
5. **Terminology:** one concept has one chosen term; identifiers and official names are intact.
6. **Register:** the translation serves the same audience and purpose as the source.
7. **Naturalness:** no avoidable calques, noun stacks, bureaucratese, or broken Russian syntax.
8. **Structure:** headings, lists, answer options, links, code, and emphasis remain usable.
9. **Typography:** relevant Russian conventions are applied consistently.

Treat repeated wording as a diagnostic signal, not an automatic error. Do not replace a precise
term merely to create variety.

### 3. Refine

Fix only issues found during the audit. Prefer active verbs and concise syntax when they improve
clarity without changing meaning. Keep passive voice, participles, gerunds, repetition, or an
evaluation when the context makes them accurate and natural. Stop when further editing would
only make the text different rather than better.

## Context Rules

### Technical documentation

- Preserve code, commands, flags, paths, file names, API fields, and product names.
- Use established Russian terminology; keep English only for identifiers, official UI labels,
  product names, or terms without a stable Russian equivalent.
- Match the document's register: formal documentation may differ from an engineering chat.
- Do not simplify away distinctions important for implementation.

### Marketing and business

- Adapt idioms and sentence structure, but preserve the strength and scope of every claim.
- Do not add superlatives, proof, urgency, calls to action, or promises absent from the source.
- Replace empty wording only when it is empty in context; retain deliberate brand voice.
- Localize conventional calls to action idiomatically: for example, `Start a free trial` is often
  «Попробуйте бесплатно», unless duration, billing, or product terminology requires a fuller form.

### Educational content

- Explain clearly and maintain the author's instructional stance.
- Preserve learning objectives, prerequisites, modality, and technical distinctions.
- Use approachable Russian without making a professional source colloquial.

### UI strings

- Respect supplied character, line, and platform constraints.
- Preserve placeholders, access keys, variables, markup, and capitalization with functional meaning.
- For numeric placeholders, use the product's pluralization mechanism or neutral syntax that does
  not hard-code an incorrect Russian noun form. Flag the issue if neither is possible.
- If no constraint is supplied, prioritize accuracy over speculative shortening.
- Mention a necessary truncation trade-off only when it materially affects the result.

### Exam and certification questions

- Make the question self-contained without introducing clues or new facts.
- Preserve modality and the distinction between correct and plausible distractors.
- Keep answer options grammatically parallel. Start them with verbs only when the source options
  describe actions; match mood, tense, and aspect where feasible. Do not force noun or value
  options into verbs.
- For one-time implementation choices written as English base-form actions, normally use parallel
  perfective infinitives: `Add / Replace / Remove / Store` → «Добавить / Заменить / Удалить /
  Сохранить».
- Remove leaked source metadata only when it is not part of the exam content.

## Mixed-Language Text

- Leave code, identifiers, commands, paths, file names, URLs, API fields, and product names intact.
- Format code elements as code when the source format supports it.
- Preserve official English UI labels when the product is not localized. Add a Russian gloss only
  if it helps the intended reader and does not violate a length constraint.
- Never mix Cyrillic and Latin lookalike characters within one word.
- Use the terminology decisions in `references/glossary-strategy.md` for technical prose.

## Output

Return only the finished translation unless the user requests commentary, alternatives, a
glossary, or the full workflow.

If a source ambiguity, apparent error, or unavoidable terminology choice materially affects the
translation, add a short section titled `Примечания переводчика` after the translation. Do not add
this section for harmless stylistic choices.

If the user asks for the full workflow, show the draft, audit findings, and final translation in
that order.
