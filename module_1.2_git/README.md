# Модуль 1.2 Знакомство с git

## Цель недели

Освоить базовые концепции системы контроля версий Git и научиться использовать основные команды для управления кодом.

## Зачем нужен Git?

Git - это незаменимый инструмент для разработчиков, который решает три ключевые проблемы: безопасность, командную работу и историю изменений. Представьте, что вы работаете над важным проектом - Git позволяет вам сохранять каждое изменение, экспериментировать с новыми идеями в отдельных ветках, и при необходимости вернуться к любой предыдущей версии кода. Когда над проектом работает команда, Git помогает синхронизировать работу всех разработчиков, избегая потери изменений и конфликтов. Более того, Git стал стандартом индустрии - его используют практически все компании, от стартапов до крупных корпораций, а ваш GitHub аккаунт становится профессиональным портфолио, демонстрирующим ваши навыки потенциальным работодателям.

## Теоретическая часть

### Что такое Git и зачем он нужен?

- Git - это система контроля версий
- Позволяет:
-   Отслеживать изменения в коде
-   Работать в команде
-   Возвращаться к предыдущим версиям
-   Создавать ветки для разных задач

### Основные концепции

1. Репозиторий
-   Локальный (на вашем компьютере)
-   Удаленный (на GitHub/GitLab)

2. Коммит
-   Снимок изменений
-   Имеет уникальный идентификатор
-   Содержит сообщение о изменениях

3. Ветка (Branch)
-    Отдельная линия разработки
-    Позволяет работать над разными задачами параллельно

## Основные команды

|Настройка Git|
|-------|
|git config --global user.name "Your Name"|
|git config --global user.email "your.email@example.com"|

|Работа с репозиторием|Описание|
|---------|----------|
|git init|создать новый репозиторий|
|git clone <url>|склонировать существующий репозиторий|
|git status|проверить статус изменений|
|git add <file>|добавить файл в индекс|
|git add .|добавить все изменения|
|git commit -m "message"|создать коммит|
|git log|посмотреть историю коммитов|

|Работа с ветками|Описание|
|---------|----------|
|git branch|посмотреть список веток|
|git branch <name>|создать новую ветку|
|git checkout <branch>|переключиться на ветку|
|git checkout -b <name>|создать и переключиться на ветку|
|git merge <branch>|объединить ветки|

|Продвинутые команды (дополнительно) | Откат изменений|
|---------|----------|
|git reset --soft HEAD~1|отменить последний коммит, сохранив изменения в индексе|
|git reset --mixed HEAD~1|отменить последний коммит, изменения останутся в рабочей директории|
|git reset --hard HEAD~1|отменить последний коммит, полностью удалив изменения|
|git revert <commit-hash>|создать новый коммит, отменяющий изменения указанного коммита|

|Изменение коммитов|Описание|
|---------|----------|
|git commit --amend | изменить последний коммит (сообщение или добавить файлы)|
|git rebase -i HEAD~3 | интерактивный rebase для изменения нескольких последних коммитов|

|Работа с историей|Описание|
|---------|----------|
|git log --oneline | компактный вывод истории|
|git log --graph | показать историю с графиком веток|
|git show <commit-hash> | показать детали конкретного коммита|
|git diff HEAD~1 | показать изменения в последнем коммите|
