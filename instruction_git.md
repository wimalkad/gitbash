# **Инструкция по работе с Git**

## Что такое Git

![Git Logo](images/git.png)
*Git - это программа для контроля версий, удобная в использовании при создании проектов*

## Создание локального репозитория

Для того чтобы создать (инициализировать) локальный репозиторий необходимо в териминале, нахоядсь в папке проекта набрать команду:

    git init

## Проверка состояния репозитория

Чтобы проверить состояние репозитория используют команду:

    git status

## Информирование об изменениях

Для того, чтобы сообщить об измненениях в рабочем файле используют команду:

    git add

## Ввод комментариев к изменнениям

Для ввода комментариев к коммиту используют:

    git commit
Эта команда также подразделяется на:
* Выполнение коммита со всеми изменениями в рабочем каталоге:
    
    **git commit -a**

* Быстрая команда создания коммита без вызова отдельного окна текстового редактор

    **git commit -m "text of message"**
* Создания коммита всех проиндексированных изменений и добавления комментария к коммиту:

    **git commit -am "text of message"**

## Отслеживание изменений

Чтобы вызвать журнал изменений используют команду:

    git log

*для удобного вывода информации, используется вариация*:

    git log --oneline

## Переключение между версиями

Для переключения между версиями используют команду:

    git checkout <hash>

Перед использованием данной команды нужно ввести интересующий вас коммит и вернуться в тот, где работем с помощью команды:
    
    git checkout master

## Отображение изменений

Чтобы показать разницу между текущим и сохраненным файлом можно воспользоваться командой:

    git diff <hash> <hash>

## Ветвления

Ветвления нужны для управления черновиками и чистовиками в Git

~~строка для проверки работы ветвления~~s


## Создание новой ветки

Для того, чтобы создать новую ветку необходимо ввести команду

    git branch <branch_name>

## Удаление ветки

Для того, чтобы удалить определенную ветку, необходимо ввести команду:

    git branch -d <branch_name>

    -d - сокращение от delete
    <branch_name> - имя ветки

## Слияние веток

Для слияния веток необходимо воспользоваться командой:

    git merge <branch_name>

## Визуализация веток

При вызове команды "git log" можно упростить просмотр ветвей, 
благодаря графическому отображению:

    git log --graph

## Переключение между ветками

Для переключения между ветками используется команда:

    git checkout <branch_name>

## Удаленные репозитории

Удаленные репозитории позволяют другим пользователям работать совместно с вами,
не имея на ПК локальных файлов репозитория, сред программирования

## Загрузка новых изменений в удаленный репозиторий

Для того, чтобы загрузить сделанные локально изменения в удаленный репозиторий нужно использовать команду:

    git push

## Выгрузка из удаленного репозитория

Для того, чтобы отправить изменения, сделанные локально в удаленный репозиторий необходимо использовать команду:

    git pull