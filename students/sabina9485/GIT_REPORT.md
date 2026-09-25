# Отчёт по Git Flow

## Что сделано

### Поток фичи (feature → develop)
1. Создала develop от main
2. Создала feature/sabina9485-intro от develop
3. Сделала 4 коммита (ABOUT.md, NOTES.md, .env.example, .gitignore)
4. Открыла PR #1: feature → develop
5. Разрешила учебный конфликт в sandbox/conflict.txt
6. Merge PR #1 в develop

### Поток hotfix (main → develop)
1. Создала hotfix/sabina9485-typo от main
2. Внесла «баг» (Helo вместо Hello)
3. Исправила опечатку
4. PR #2: hotfix → main, merge
5. Обязательно влила hotfix в develop
6. Удалила hotfix-ветку

## Роли веток Git Flow

| Ветка | Откуда | Куда | Зачем |
|-------|--------|------|-------|
| main | — | — | Боевая/релизная линия |
| develop | от main при старте | — | Черновик следующего релиза |
| feature/* | от develop | в develop | Одна фича/задача |
| release/* | от develop | в main и develop | Подготовка релиза |
| hotfix/* | от main | в main и develop | Срочный фикс прода |

## Итоговый граф

См. `git log --oneline --graph --all`
