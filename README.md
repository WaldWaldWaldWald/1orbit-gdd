# 1ORBIT GDD — контекст для Claude

## Что это

Git-репозиторий с правилами и знаниями для AI-ассистента проекта 1ORBIT. Claude Code / Cowork автоматически загружает `CLAUDE.md` и `.claude/rules/` при старте каждой сессии.

## Структура

```
CLAUDE.md                    — главный файл (загружается первым)
.claude/
  settings.json              — настройки Claude Code
  rules/
    01-workflow.md            — порядок работы
    02-types-and-hierarchy.md — типы страниц и дерево ГДД
    03-text-style.md          — правила текста
    04-protection.md          — защита контента и инварианты
    05-parameters.md          — параметры и формулы
    06-balance.md             — баланс и таблицы
    07-dor-dod.md             — чек-листы готовности
knowledge/
  mechanics-registry.md       — реестр всех механик
  decisions-log.md            — лог дизайн-решений
  known-errors.md             — паттерны ошибок Claude
```

## Как использовать

1. Склонируй репо локально
2. Открой Claude Code / Cowork из папки `1orbit-gdd/`
3. Claude автоматически загрузит все правила
4. Работай с ГДД как обычно — Claude будет следовать правилам

## Обновление

- **После каждой сессии** Claude обновляет файлы в `knowledge/`:
  - Новые ошибки → `known-errors.md`
  - Новые решения → `decisions-log.md`
  - Новые/изменённые механики → `mechanics-registry.md`
- **При изменении правил** в Confluence → обнови соответствующий файл в `.claude/rules/`
- Коммить изменения в Git после каждой рабочей сессии

## Контент ГДД

Контент (страницы механик, каталоги, фичи) живёт в Confluence:
- Корень ГДД: https://innowald.atlassian.net/wiki/spaces/inno/pages/141000705
- Контекст (правила): https://innowald.atlassian.net/wiki/spaces/inno/pages/141099009
- Баланс (числа): https://docs.google.com/spreadsheets/d/1Z2NQQoNjrdqmnXBi_qqt4fgQ2GZ_eP6uqP1F_E8Bmrg
