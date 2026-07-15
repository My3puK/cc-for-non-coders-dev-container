# Terminology and Glossary Strategy

Use this reference for technical, long, repetitive, or multi-document translations.

## Decision order

Choose a term by checking, in order:

1. the customer's approved glossary or translation memory;
2. official Russian product documentation and localized UI;
3. an established term in the target professional community;
4. a clear Russian equivalent that preserves the distinction;
5. the English term when no stable Russian equivalent exists.

Once chosen for a concept, use the term consistently. Do not introduce synonyms merely to avoid
repetition. A different translation is valid only when the English word denotes a different
concept or the context changes its meaning.

## Build a glossary when

- the source is longer than two pages;
- it belongs to a document series;
- it uses domain-specific or product-specific terminology;
- one ambiguous term appears at least five times;
- several translators or translation sessions must remain consistent.

Record the English term, chosen Russian equivalent, context, protected form, and exceptions.

## Canonical software terms

These are defaults, not substitutes for an approved customer glossary.

| English | Russian prose | Keep in English when | Notes |
|---|---|---|---|
| skill | навык | It is an identifier or official untranslated UI label. | Do not use «скилл» in neutral documentation. |
| connector | коннектор | `Connector` is an official label. | Use «интеграция» only when the concept is genuinely broader than a connector. |
| workflow | рабочий процесс | It is code, an identifier, or an official UI label. | In automation products, «сценарий» is acceptable only when that is the product's established concept. |
| trigger | триггер / условие запуска | It is code, an event name, or an official UI label. | «Триггер» is established in technical prose; use «условие запуска» for a broader audience when accurate. |
| workspace | рабочее пространство | It is an official UI label or identifier. | A product may use «проект» as a distinct concept; follow its glossary. |
| description field | поле `description` / поле описания | `description` is the literal field name or identifier. | Preserve the code form when referring to YAML, JSON, or an API schema. |
| version control | управление версиями | It is an official feature name or identifier. | Use «система контроля версий» when the source means a VCS such as Git. |
| tool | инструмент | `tool` is an API value, type, field, or identifier. | `tool call` → «вызов инструмента» in prose. |
| hook | хук | `hook` is code, an API value, or an identifier. | For a nontechnical audience, «обработчик» may be clearer if accurate. |
| middleware | middleware | It is an API or framework term. | Use «промежуточный обработчик» or «промежуточный слой» only when it describes the architecture precisely. |
| endpoint | API-эндпоинт | It is code or an official label. | «Конечная точка» is acceptable in a customer glossary but should not alternate with «эндпоинт». |
| frontmatter | YAML-шапка | It is code or a field name. | In formal prose, «блок YAML-метаданных» may be preferable. Pick one form per document. |
| progressive disclosure | постепенная подача / поэтапное раскрытие | It is an official design-pattern name. | Avoid «прогрессивное раскрытие» unless it is the approved product term. |
| composability | сочетаемость / модульность | It is an official architecture term. | Choose by meaning: ability to combine components is «сочетаемость»; component design may be «модульность». |
| distribution | публикация / размещение / доставка / развёртывание | It is an official feature name. | Translate by function; there is no universal equivalent. |
| pipeline | CI/CD-пайплайн; конвейер обработки данных | It is code or an official label. | Do not alternate forms for one pipeline. |
| conversation | диалог | It is code or an API field. | In an LLM context, avoid «разговор» unless the product itself uses it. |
| session | сеанс / сессия | It is code or an API field. | Choose according to the product glossary and keep it stable. |
| extraction schema | схема извлечения данных | It is an identifier or official schema name. | Do not force the hybrid «extraction-схема» without product evidence. |
| severity | уровень критичности | It is the field or enum value `severity`. | Preserve enum members exactly. |
| deploy | развернуть | It is a command or identifier. | Informal team chat may use «задеплоить» if that matches the source register. |
| publish | опубликовать | It is a command or identifier. | Do not replace with «развернуть» unless deployment is meant. |
| bundle | комплект / набор / пакет | It is code, an identifier, or an official product term. | Choose by what is bundled; do not default to «бандл» in neutral prose. |
| reference file | справочный файл | It is an official label or identifier. | «Файл-пример» is different and should not replace it. |
| asset | ресурс / материал | It is code, a directory name, or an official label. | In design and web projects, the approved term may be «ассет»; keep it only when the audience expects it. |
| kebab-case | kebab-case | It is a formatting term. | Keep the established Latin form and explain it only when the audience needs a gloss. |
| MCP server | MCP-сервер | `MCP server` is an identifier or official UI label. | Keep MCP in Latin script and translate the generic noun. |

## Protected English forms

Keep product and organization names, standard abbreviations, formats, code, identifiers, and
unlocalized UI labels in their official form: Codex, Claude, MCP, Docker, GitHub, API, SDK, CLI,
JSON, YAML, HTTP, `SKILL.md`, `severity`, and `pip install`.

Translate surrounding generic words naturally: «MCP-сервер», «API-клиент», «JSON-файл».
Never replace Latin characters inside an identifier with Cyrillic lookalikes.

## Resolve drift

When a chosen translation proves inaccurate:

1. update the glossary decision;
2. replace every instance that denotes the same concept;
3. verify that code and official labels were not altered;
4. re-read affected sentences for grammar and meaning;
5. record the context-dependent exception instead of creating unexplained variation.

## Do not confuse consistency with uniform substitution

One English word may have different meanings. Translate by concept:

- `issue`: «задача» in a tracker, «замечание» in an audit, «проблема» in general prose;
- `process`: «обрабатывать» as a verb, «процесс» as a noun;
- `handle`: «обрабатывать» requests, «поддерживать» formats, «дескриптор» as a programming noun;
- `implement`: «реализовать» a function, «внедрить» a solution;
- `control`: «управлять» a system, «контролировать» compliance, «элемент управления» in a UI.

Consistency applies to the same concept, not to the same English spelling in every context.
