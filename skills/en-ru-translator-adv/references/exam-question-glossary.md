# AI and Software Exam Translation

Use this reference for certification and exam questions about Codex, Claude, LLMs, APIs, software
architecture, and agent workflows. Apply an official exam glossary first if one is supplied.

## Structure

| English field | Russian field |
|---|---|
| Question | Вопрос |
| Options | Варианты ответа |
| Correct Answer | Правильный ответ |
| Explanation | Пояснение / Комментарий |
| Source | Источник |
| Section | Раздел |
| Scenario | Сценарий |

Preserve the source schema and field order unless the user requests another format. Remove internal
filenames, duplicate numbering, or editorial notes only when they are source artifacts rather than
exam content.

## Core terminology

| English | Russian prose | Protected form or note |
|---|---|---|
| extraction schema | схема извлечения данных | Keep an official identifier unchanged. |
| severity | уровень критичности | Keep the field `severity` and its enum values unchanged. |
| companion field | сопутствующее поле | Use the official schema term if supplied. |
| correct answer | правильный ответ | «Корректный» may describe validity, not correctness in a test. |
| explanation | пояснение / комментарий | Match the source field label. |
| deterministic | детерминированный | |
| probabilistic | вероятностный | |
| enforcement | обеспечение / контроль соблюдения | Choose by mechanism and object. Avoid literal «принуждение» unless force is actually meant. |
| human escalation | передача оператору / эскалация на оператора | Make the human role explicit when `agent` could be confused with an AI agent. |
| refund | возврат средств | |
| validation | валидация / проверка | Use «валидация» for a defined technical stage; «проверка» for the general action. |
| classification | классификация | |
| agentic | агентный | |
| workflow | рабочий процесс | Keep code and official UI labels unchanged. |
| option | вариант ответа | |
| prerequisite | предусловие / обязательное условие | Use «предусловие» in program logic. |
| tool | инструмент | Keep `tool` in code or API values. |
| tool use | использование инструментов / вызов инструмента | Distinguish the general capability from one concrete call. |
| tool call | вызов инструмента | |
| hook | хук | Keep `hook` in code or identifiers. |
| callback | функция обратного вызова / колбэк | Keep code and identifiers unchanged; use «колбэк» only for an appropriate technical audience. |
| middleware | middleware / промежуточный обработчик | Follow the framework and audience glossary. |
| endpoint | API-эндпоинт | Keep endpoint names and identifiers unchanged. |
| system prompt | системный промпт | |
| user prompt | пользовательский промпт | |
| token | токен | Keep code, field names, and literal token values unchanged. |
| context window | контекстное окно | Use an approved product term if different. |
| few-shot | few-shot / с несколькими примерами | Preserve an official methodology label; explain it for a broader audience if needed. |
| zero-shot | zero-shot / без примеров | Preserve an official methodology label; do not confuse it with zero input. |
| chain-of-thought | цепочка рассуждений / chain-of-thought | Follow the source and product terminology; do not expand hidden reasoning absent from the source. |
| streaming | потоковая передача / стриминг | Choose the formal or engineering register; keep API values unchanged. |
| batch | пакетная обработка / пакет | Keep `batch` in code, API values, or official labels. |
| scratchpad | черновик / scratchpad | In compounds, use the established product form, such as `scratchpad`-файл, only when documented. |
| overhead | накладные расходы / служебная нагрузка | Choose financial, computational, or operational meaning. |
| burden | нагрузка | Avoid literary «бремя» in neutral technical prose. |
| misuse | использование не по назначению / неправильное использование | Use «злоупотребление» only when intentional abuse is actually meant. |

Keep common abbreviations and formats unchanged: API, SDK, REST, HTTP, JSON, XML, YAML, CSV, RAG,
MCP, CLI. Keep data types and values as code when they refer to schema syntax: `enum`, `string`,
`boolean`, `integer`, `float`, `null`.

## Context-dependent terms

- `issue`: «задача» in a tracker, «замечание» in an audit, «проблема» generally.
- `pipeline`: «CI/CD-пайплайн» in DevOps; «конвейер обработки данных» in data processing.
- `conversation`: «диалог» in an LLM context; keep an API field unchanged.
- `session`: «сеанс» or «сессия» according to the product glossary.
- `implement`: «реализовать» a function; «внедрить» a solution.
- `handle`: «обрабатывать» requests; «поддерживать» formats; «дескриптор» as a programming noun.
- `safely`: «безопасно» or «без побочных эффектов» according to the actual risk.

## Question integrity

1. Preserve `must`, `should`, `may`, `can`, negation, bounds, and comparative force.
2. Keep the stem self-contained using only context present in the source item.
3. Preserve distractor plausibility; do not explain or normalize one option more than the others.
4. Keep options grammatically parallel, including verb mood, tense, and aspect. For one-time
   implementation choices, translate `Add / Replace / Remove / Store` with parallel perfective
   infinitives: «Добавить / Заменить / Удалить / Сохранить».
5. Start options with verbs only when the source options describe actions.
6. Preserve code, fields, enum values, model names, API names, and version numbers.
7. Keep the explanation's certainty and reasoning; do not add a rationale absent from the source.
8. Flag a materially incomplete or contradictory source instead of inventing missing context.

Example of preserved modality:

- `What should you add?` → «Что следует добавить?»
- `What must the schema include?` → «Что должна содержать схема?»
- `Which option may reduce latency?` → «Какой вариант может сократить задержку?»
