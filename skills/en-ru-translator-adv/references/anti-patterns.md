# English-to-Russian Translation Anti-Patterns

Use this reference to diagnose a draft that sounds literal, repetitive, or machine-translated.
Apply each correction only when it preserves the source meaning and register.

## Contents

- [Calques](#calques)
- [Machine-writing markers](#machine-writing-markers)
- [False friends](#false-friends)
- [Technical prose](#technical-prose)
- [Grammar and structure](#grammar-and-structure)
- [Repetition](#repetition)
- [Lists](#lists)
- [Register](#register)
- [Exam questions](#exam-questions)
- [Final audit](#final-audit)

## Calques

| Literal wording | Natural options, depending on context |
|---|---|
| Это имеет смысл. | Это логично. / Понятно. / Разумно. |
| Я имею проблему. | У меня проблема. / Я столкнулся с проблемой. |
| В конце дня... | В итоге... / К концу дня... when the literal day is meant. |
| Иметь место | Происходить / встречаться / быть, according to meaning. |
| Оказывать влияние | Влиять |
| Находиться в процессе настройки | Настраиваться / сейчас настраиваем |
| Иметь возможность | Мочь / можно |
| Быть вовлечённым | Участвовать, if participation is meant. |
| Нести ответственность за | Отвечать за, unless legal wording requires the fuller form. |
| Получить максимум от | Использовать на полную / извлечь пользу |
| Низкий порог входа | Легко начать / легко освоить, unless the term is established for the audience. |

Do not replace a phrase mechanically. `At the end of the day` may literally refer to a time, and
`responsible for` may require a formal legal equivalent.

## Machine-writing markers

Watch for frequent but context-poor equivalents:

| English | Risky default | Better contextual choices |
|---|---|---|
| delve | погрузиться | изучить / разобраться / рассмотреть подробнее |
| landscape | ландшафт | ситуация / среда / сфера / рынок |
| tapestry | гобелен / полотно | сочетание / разнообразие / картина |
| testament | свидетельство | показывает / подтверждает, if the evidence supports it |
| underscore | подчёркивать | показывать / выделять / напоминать |
| pivotal | поворотный | важный / решающий |
| foster | способствовать | развивать / поддерживать / создавать условия |
| harness | обуздать | использовать / задействовать |
| navigate an abstract field | навигировать | ориентироваться / разбираться |
| serve as | служить чем-либо | быть / использоваться как |

These words are not forbidden. Use the precise equivalent when the literal image or established
term is intentional.

## False friends

The previous version contained a broad false-friends list. Retain the entries below because they
are common and semantically stable, but choose the final wording by context.

| English | Risky automatic choice | Contextual Russian equivalents |
|---|---|---|
| accurate | аккуратный | точный / достоверный; «аккуратный» only when neatness or careful execution is meant |
| actual | актуальный | фактический / реальный / действительный; «актуальный» only when current relevance is meant |
| realize | реализовать | понять / осознать; «реализовать» when implementing or making something real |
| control | контролировать | управлять / регулировать / контролировать, according to the relationship |
| originally | оригинально | изначально / первоначально; «оригинально» when creatively or unusually is meant |
| prospect | проспект | перспектива / потенциальный клиент / предполагаемый результат, according to context |
| sympathetic | симпатичный | сочувствующий / понимающий / благожелательный |
| data | дата | данные |
| fabric | фабрика | ткань / материал / структура, according to context |
| magazine | магазин | журнал; «магазин» only when a technical storage or feed device is meant |
| decade | декада | десятилетие; «декада» only for a ten-day period or an established specialist term |
| revision | ревизия | редакция / версия / пересмотр / доработка; «ревизия» for an inspection or audit |
| technique | техника | метод / приём / способ; «техника» when equipment, skill, or execution technique is meant |
| record | рекорд | запись / документ / показатель / учётная запись; «рекорд» for the best result |

Do not treat the middle column as a ban. A false friend becomes correct when the context genuinely
has that meaning.

## Technical prose

Common failures include:

- translating official identifiers or code;
- copying English noun stacks into Russian;
- using several Russian terms for one technical concept;
- preserving English syntax after translating every word;
- replacing a precise technical term with a vague everyday word;
- applying one translation to every sense of an English word.

Examples:

| English | Avoid | Prefer |
|---|---|---|
| control skill management and execution | контроль над управлением и выполнением навыков | управлять навыками и запускать их |
| YAML frontmatter | YAML-преамбула | YAML-шапка / блок YAML-метаданных |
| packaged into a folder | упакованный в папку | собранный в папке / папка с... |
| two ways through this guide | два пути через руководство | два способа работать с руководством |
| progressive disclosure | прогрессивное раскрытие | постепенная подача / поэтапное раскрытие |

Use [glossary-strategy.md](glossary-strategy.md) for canonical software terms. Do not create a
different local term merely for stylistic variety.

## Grammar and structure

### Noun stacks

Turn hidden actions into verbs when it improves clarity:

- «осуществление внедрения» → «внедрение» or «внедрить»;
- «проведение анализа» → «анализ» or «проанализировать»;
- «предоставление доступа» → «дать доступ»;
- «обеспечение выполнения требования» → «обеспечить соблюдение требования» or a more direct verb.

Do not force a verb if the noun names a defined process, UI element, legal concept, or technical
artifact.

### Passive voice

Avoid passive voice when it hides a relevant actor or follows English syntax mechanically. Keep it
when the actor is unknown, irrelevant, or intentionally backgrounded.

- Heavy: «Решение было принято командой» → «Команда решила».
- Valid state: «Доступ запрещён политикой организации».
- Unknown actor: «Файл был удалён до начала проверки».

### Pronouns

Drop English possessive pronouns when Russian context already makes ownership clear, but preserve
them when they distinguish people, accounts, teams, or data.

## Repetition

Repeated sentence openings, transitions, or empty templates may make a draft mechanical. Vary or
merge them only if the change preserves emphasis and structure.

Do not apply a numeric ban such as “never repeat a word twice within 15 words.” Repetition is often
necessary for:

- technical terminology;
- legal precision;
- parallel instructions;
- deliberate rhetoric;
- avoiding an ambiguous pronoun.

Treat repetition as a prompt to inspect, not an instruction to replace. Vary surrounding syntax
before replacing a canonical term.

## Lists

Check that items have compatible grammatical roles and answer the lead-in correctly.

Bad:

```text
Чему вы научитесь:
- Технические требования
- Использовать шаблоны
```

Good:

```text
Чему вы научитесь:
- понимать технические требования;
- использовать шаблоны.
```

Do not force every list item to start with a verb. Noun lists, values, labels, and factual answer
options should remain nouns or values when that matches the source. Follow the format-sensitive
punctuation rules in [typography.md](typography.md).

## Register

Do not replace every anglicism automatically. Decide whether it is:

- an avoidable borrowing: «таск» → «задача» in neutral documentation;
- an established general term: «стартап», «маркетинг», «дизайн»;
- a professional term appropriate to the audience: «CI/CD-пайплайн»;
- code, an identifier, or an official label that must remain unchanged;
- deliberate slang in an informal source whose tone should be preserved.

Avoid bureaucratese that the source does not require: «данный», «в целях», «на сегодняшний день»,
«осуществлять», and chains of nominalizations. Preserve formal wording when it carries legal,
regulatory, or contractual force.

## Exam questions

Avoid:

- a question that depends on omitted context;
- losing `should`, `must`, `may`, or another modal distinction;
- rewriting distractors so aggressively that the correct answer becomes obvious;
- forcing action verbs onto answers that are values, terms, or factual statements;
- leaking source filenames, internal numbering, or editorial notes into exam content;
- translating enum values, fields, or API identifiers;
- changing the degree of certainty in the explanation.

Example:

- Incomplete: «Что следует добавить?»
- Self-contained: «Что следует добавить в схему, чтобы сохранить исходное значение `severity`?»

Add context only when it is available elsewhere in the source item. Do not invent missing facts to
make a question self-contained; flag a materially incomplete source instead.

## Final audit

Before accepting a stylistic correction, verify:

1. The new wording makes the same claim.
2. Certainty, modality, range, and scope are unchanged.
3. No evidence, benefit, actor, or consequence was added.
4. A canonical technical term was not replaced by a decorative synonym.
5. The result matches the target audience rather than a universal notion of “good Russian.”
