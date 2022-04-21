# Основные команда по GIT
## Первый запуск
https://git-scm.com/

*узнаем текущию версию*
> git --version   

*иницидизируем git*
> git init

**Представляемся**
> git config --global user.name "Name"

> git config --global user.email "mail@mail.ru"
---
## Основные команды запись
*текущее состояние сохранения*
> git status

*добавляем файл*
> git add '.\hello world.md' 

*или все файлы папки*
> git add .

*коммитим то что сохоанили*
> git commit -m "Создали новый файл"

*поиск разницы текущего состояния и сохраненного*
> git diff

## Основные команды в истории

*История* 
> git log

    q - выйти  enter - продолжить

*возврат в коммиту*
> git checkout 8379

    достадочно 4 символа

*возврат в актуальное состояние*
> git checkout master

## Основные команды Ветки

*новая ветка*
> git checkout -b "gitMaster"

*вернуться на ветку*
> git checkout  master 

*показываем ветки*
>git branch

*создаем ветку*
>git branch NAME

*вернуться на ветку*
>git checkout  master

*слияние веток*
>get merge NAME

*удаление ветк*
>git branch -d NAME 
(-d на это указывает)

## Работа с удаленным репозиторием
*клонируем себе удаленный репозиторий*
>git clone URL

### Привязка локального репозитория к удаленному
*к чему привязываем*
>git remote add origin https://github.com/Vestibolog/test.git
*переименовываем ветку в main*
> git branch -M main
*загружает в гитхаб ветку main*
> git push -u origin main


*отправить в github*
> git push

*принемает из пшерги(+ делает merge)*
> git pull


# Последовательность действий для работы с github из лекции
1. Делаем fork репозитория
2. Делаем git clone клона репозитория
>git clone URL
3. создаем ветку с предлагаемыми изминениями
>git checkout -b NAME
4. делаем изминения только в этой ветке
> git add FILEMANE

> git commit -m "Создали новый файл"
5. делаем push
> git push
6. появляетс возможность COMPARE & Pull

git push -u orign master

# Последовательность действий для работы с github из семинара
1. git init
2. git add FILEMANE
3. git remote add origin URL
4. git commit -m "git init"
5. git push -u origin master

*новое задание в новой ветке*
6. git checkout -b NAME
7. git push -u origin NAME

## Вспомогательные команды
> clear

> cd

> ls - список фалов

> cat hello\ world2.md - инфо про файл

> touch read.md - создать файл

> rm name.md - удалить файл