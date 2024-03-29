# Подсказка по Git

### Общие подсказки:
* **При многостраничном просмотре, например командами *git log* или *git diff*, для выхода нажать клавишу *[q]*.**
* **Для ввода номера коммита достаточно ввести первые четыре символа.**
* **Для того, чтобы Git игнорировал определенные файлы в папке необходимо создать файл .gitignore и вписать туда эти файлы.**

### Получить помощь:
```sh
git --help
```
### Получить краткую подсказау по команде:
```sh
git <some_command> -h
```
### Получить развернутую подсказку по команде:
```sh
git <some_command> --help
```
### Создание репозитория:
```sh
git init
```
### Проверка состояния репозитория:
```sh
git status
```
### Добавить файл в индекс для коммита:
```sh
git add file_name
```
### Добавить индекс все файлы в папке (даже которых нет в репозитории) для коммита:
```sh
git add -А  
git add --all
git add .
```
### Удалить файл из индекса и репозитория:
```sh
git rm file_name
```
### Отменить изменения в еще не индексированном файле до последнего закоммиченного состояния:
```sh
git restore file_name
```
### Отменить изменения в файле, уже добавленном для индексирования:
```sh
git restore --staged file_name
```
### Выполнить коммит в репозиторий с соответствующим сообщением:
```sh
git commit -m "Message for commit"
```
### Выполнить коммит в репозиторий всех измененных файлов в директории, не добавленных через команду *git add*, но только если они уже есть в репозитории:
```sh
git commit -a
```
### Просмотреть журнал репозитория:
```sh
git log
```
### Просмотреть журнал репозитория в сокращенном виде:
```sh
git log --oneline
```
### Просмотреть журнал с показом веток коммитов:
```sh
git log --graph
```
### Перейти в состоянию репозитория с номером hash_number:
```sh
git checkout hash_number
```
### Перейти к последнему состоянию репозитория ветки master:
```sh
git checkout master
```
### Перейти к последнему состоянию репозитория ветки branch_name:
```sh
git checkout branch_name
```
### Восстановить файл к определенному состоянию, можно использовать имя ветки или хеш-номер коммита:
```sh
git checkout number|name file_name
```
### Восстановить все файлы к определенному состоянию, можно использовать имя ветки или хеш-номер коммита:
```sh
git checkout number|name *
```
### Показывает разницу между текущим сохраненными файлами и последним состоянием репозитория: 
```sh
git diff
```
### Показывает разницу между текущими сохраненными файлами и состоянием репозитория с номером hash_number:
```sh
git diff hash_number
```
### Показать ветки:
```sh
git branch
```
### Создать ветку branch_name:
```sh
git branch branch_name
```
### Удалить полностью слитую ветку branch_name:
```sh
git branch -d branch_name
```
### Слить ветку branch_name с текущей веткой:
```sh
git merge branch_name
```

### Для добавления текущего репозитория на Github необходимо выполнить следущие команды (инструкция с Github):
```sh
git remote add origin http://репозиторий
git branch -M main
git push -u origin main
```
### Склонировать удаленный репозиторий на комп:
```sh
git clone http://репозиторий
```
### Отправить измененния в удаленный репозиторий:
```sh
git push
```
### Получить изменения с удаленного репозитория:
```sh
git pull
```