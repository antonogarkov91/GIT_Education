# Инструкция для работы с Git и удаленными репозиториями

## Что такое Git?
Git - это одна из реализаций распределённых систем контроля версий, имеющая как и локальные, так и удалённые репозитории. Является самой популярной реализацией систем контроля версий в мире.
## Подготовка репозитория
Для создания репозитория необходимо выполнить команду 
```sh
git init
``` 
в папке с репозиторием и у Вас создастся репозиторий (появится скрытая папка .git)

## Создание коммитов

### Git add
Для добавления изменений в коммит используется команда 
```sh 
git add
```

 Чтобы использовать команду *git add* напишите *git add <имя файла>*

 ### Зафиксировать изменения
 ```sh
 git commit -m "Message text"
 ```

### Просмотр состояния репозитория
Для того, чтобы посмотреть состояние репозитория используется команда 
```sh
*git status*
```
 Для этого необходимо в папке с репозиторием написать *git status*, и Вы увидите были ли изменения в файлах, или их не было.

### Процесс работы с Git
Не стоит после каждого изменения файла делать commit. Чаще всего их создают, Когда:
* Создан новый функционал
* Добавлен новый блок на верстке
* Исправлены ошибки по коду
* Вы завершили рабочий день

### Просмотр истории коммитов
Для отображения отправленных снимков состояния и просмотра истории проекта, а также поиска конкретных изменений выполняется команда:
```sh
git log
```
Для отображения списка коммитов с комментариями используется команда:
```sh
git log --oneline
```
### Перемещения в репозитории
Команда:
```sh
git checkout <branch_name> or <ID commit>
```
используется, чтобы обновлять состояние репозитория до определенной точки в истории проектов.

### Отображение всех веток
```sh
git branch
```

### Создание новых веток
Команда
```sh
git branch <branch_name>
```
### Удаление веток
```sh
git branch -d <branch_name>
```