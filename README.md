# *Инструкция для работы с Git и удалёнными репозиториями*
![для начинающих](image8_0e61d0dad8.png)
***
## Что такое Git?
Git - это одна из реализаций распределённых систем контроля версий, имеющая как и локальные, так и удалённые репозитории. Является самой популярной реализацией систем контроля версий в мире.
>>[Репозиторий](https://ru.wikipedia.org/wiki/%D0%A0%D0%B5%D0%BF%D0%BE%D0%B7%D0%B8%D1%82%D0%BE%D1%80%D0%B8%D0%B9 "Википедия") — место, где хранятся и поддерживаются какие-либо данные. 

У Git есть три основных состояния, в которых могут находиться ваши файлы: изменён (modified), индексирован (staged) и зафиксирован (committed)
Механизм, которым пользуется Git при вычислении хеш-сумм, называется SHA-1 хеш. Это строка длиной в 40 шестнадцатеричных символов (0-9 и a-f), она вычисляется на основе содержимого файла или структуры каталога.

## Подготовка репозитория
Для создание репозитория необходимо выполнить команду *git init*  в папке с репозиторием и у Вас создаться репозиторий (появится скрытая папка .git)

## Создание коммитов

### Git add
Для добавления измений в коммит используется команда *git add*. Чтобы использовать команду *git add* напишите *git add <имя файла>*

### Просмотр состояния репозитория
Для того, чтобы посмотреть состояние репозитория используется команда *git status*. Для этого необходимо в папке с репозиторием написать *git status*, и Вы увидите были ли измения в файлах, или их не было.

### Создание коммитов
Для того, чтобы создать коммит(сохранение) необходимо выполнить команду *git commit*. Выполняется она так: *git commit -m "<сообщение к коммиту>*. Все файлы для коммита должны быть ***ДОБАВЛЕНЫ*** и сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО***.

## Перемещение между сохранениями
Для того, чтобы перемещаться между коммитами, используется команда *git checkout*. Используется она в папке с репозиторием следующим образом: *git checkout <номер коммита>*

## Журнал изменений
Для того, чтобы посмотреть все сделанные изменения в репозитории, используется команда *git log*. Для этого достаточно выполнить команду *git log* в папке с репозиторием

## Ветки в Git

>### Создание ветки

Для того, чтобы создать ветку, используется команда *git branch*. Делается это следующим образом в папке с репозиторием: *git branch <название новой ветки>*

>### Слияние веток

Для того чтобы добавить ветку в текущую ветку используется команда *git merge <name branch>*

При попытке объединить ветки, в которых изменена одна и та же часть того же файла, Git не сможет сделать выбор между версиями. В таком случае операция останавливается прямо перед созданием коммита слияния, чтобы пользователь вручную разрешил конфликты.

*При обнаружении конфликта выполните команду git status, чтобы увидеть, какие файлы необходимо исправить.*

>### Удаление веток
Для удаления ветки ввести команду "git branch -d 'name branch'"

## Работа с удаленным репозиторием
Чтобы забрать себе в аккаунт GitHub копию репозитория нужно нажать кнопку *"Fork"*.
Для клонирования репозитория на локальный компьютер, используем команду **"git clone"** и копируем URL-адрес. 
Чтобы отправить измененный репозиторий в GitHub, используем **"git push"**.
Кнопка *"Compare & pull request"* используется, чтобы предложить владельцу репозитория свои изменения.
Команда **"git pull"** используется для получения информации об изменениях.  

***
![Просто картинка](testpicture.jpg)