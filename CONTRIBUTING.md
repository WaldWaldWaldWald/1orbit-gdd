# Как вносить изменения

## Кто может вносить изменения

- **Гейм-дизайнер** — любые изменения в правилах и knowledge/
- **Claude (AI)** — только knowledge/ (автоматическое обновление после сессии)

## Процесс для людей

1. Создай ветку от `main`
2. Внеси изменения
3. Создай PR с описанием: что изменено и почему
4. После ревью — merge в `main`

## Процесс для Claude

Claude автоматически предлагает обновления `knowledge/` после сессии:
- Новые ошибки → `knowledge/known-errors.md`
- Новые решения → `knowledge/decisions-log.md`
- Новые механики → `knowledge/mechanics-registry.md`

Claude НЕ меняет `.claude/rules/` и `CLAUDE.md` без явного запроса гейм-дизайнера.

## Правила коммитов

Формат сообщения: `[тип] краткое описание`

Типы:
- `[rules]` — изменение правил (.claude/rules/)
- `[knowledge]` — обновление базы знаний (knowledge/)
- `[config]` — изменение конфигурации (.claude/settings.json, .gitignore)
- `[docs]` — изменение README, CONTRIBUTING
