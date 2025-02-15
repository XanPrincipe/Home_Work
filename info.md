# Что такое git 

*Это система контоля версий ,которая позволяет сохранить ваши файлы и их историю изменений*

# Подготовка репозитория
*Перед началом нужно прдставиться репозиторию:*
* git config user.name "name"
* git config user.mail "mail@m.com"

*Можно прописать name и email локально:*
* git config --local user.name 
* git config --local user.email 

# Создание сохранений 
*Для того,чтобы сохранить наши изменения ,нужно добавить их через команду add:*

* git add file_name

    Добавит к отслеживанию файл с именем file_name

* git add .

    Добавит все файлы

*После того,как добавили фалы дял отслеживания ,нужно зафиксировать их изменения*

* git commit -m "massage"

*Если файл был не внесен с помощью каманды add хотя бы один раз, то можно дальше просто использовать*

* git commit -a -m "massage"

# Проверка состояния репозитория
*Для отслеживания состояния репозитория существует много команд:*
* git status

    Показывает незакомиченные изменения
* git log

    Показывает историю изменения
* git diff

    Показывает разницу между текущими изменениями и теми что уже закомичены
* git diff branch_name

    Показывает разницу между  изменениями в текущей ветки и в ветке branch_name
* git show

    Показывает изменения для последнего комита
* git show commit_tag

    Показывает изменения внесенные в этом комите с тегом commit_tag

# Перемещение между сохранениями (обязательно про возрат в конце на конце ветки master)
Команды:
* git checkout commit_tag

    Позволяет перейти к изменениям в коммите с текгом commit_tag
* git checkout master

    Вернет вас к актуальному состоянию(перейдет на ветку master)

# Журнал изменений (git log)
*Поаказывать историю коммитов:*
* git log

* git log --graph
    Показывает визуально историю веток
     
# Ветки в git
*Команды для работы с ветками:*
* git branch

    Показывает все ветки
* git branch branch_name

    Создает новую ветку с именем branch_name

* git checkout branch_name

    Перемещает на ветку branch_name

# Слияние веток и решение конфликтов
* git merge branch_name
    Позволяет влить ветку branch_name в текущую

*В случае возникновения конфликта нужно вручную исправить несовпадающие изменения и сделать коммит с этим конфликтом*

# Удаление веток

* git branch -d branch name

    Удаляет ветку с именем branch_name

# Инструкция по работе с git 

1. Задать имя и почту

    * git config user.name "name"
    * git config user.mail "mail@m.com"

2. Создать репозиторий 
   
    * git init

3. Работа с репозиторием
    
    1. Работать с файлами:
        * git add 
        * git commit
    2. Смотреть состояние репозитория
        * git status
        * git log
        * git diff
## git status
*Показывает текущее состояние репозитория*

# git add
*Добавляет файл к коммиту*

Команды:
* git add  file_name

    Добавляет файл с именем file_name к следующему коммиту

* git add .

    Добавляет все файлы к следующему коммиту

## git coomit 
*Фиксирует наши изменения*

Команды:

* git commit -m "massage"

    Фиксирует отмеченные файлы и добавляет к ним комментарий "massage"

* git commit -a -m "massage"

     Фиксирует все файлы и добавляет к ним комментарий "massage"

## git log 

*Показывает историю изменений* 

## git checkout

*Позволяет перейти между коммитами*

## git checkout master

*Позволяет вернуться к актуальному состоянию*

## git diff

*Показывает отличия текущей версии от закомиченной*

## --info
*Тег,который выдает справку о команде,к которой был применен*

Примеры:
* git status --info
* git commit --info

## git remote

*Эта команда показывает имя удаленного репо, если такой имеется в наличии*

## git remote add

*Добавление удаленных репозиториев под короким именем*

## git push

*Команда git push говорит Git, куда отправить наши изменения, когда все готово*

## git pull

* git pull origin master

*Забираем изменения из ветки (master) на удаленном сервере (origin) и проводим слияние с активной веткой*

## git clone

*По url создаем локальный репозиторий, склонировав удаленный, например, с gitHub*


