# Инструкци по работе с Git.
 
## Что такое Git?

***Git*** - самая популярная реализация распредленной системы контроля версий( версеонность поддерживается на сервере, и у каждого клиента)ю Самой распростроненно   реализацией ***Git*** является (*Git*)[http://github.com]


## Подготовка репозитория
Для создание репозитория используется команда *git init*ю Для этого необходимо открыть в терминале папку с будующим репозиторием и написать *git init*.
 
## Создание коммит
ДЛя создания новой фиксации(коммита) импользется команда 8git commit*ю Для этого в терминале с папкой-репозиторием пишем *git commit -m "<сообщение к комииту>". Сообщение к коммиту посать ***ОБЯЗАТЕЛЬНО!!!***

### Добавление файлов к коммиту
Для добавление файлов к новому коммиту изпользуется комнада *git add*. Используется она следующим образом: в терменале с папкой-репозиторием пишем *git add <название файла>*.

## Перемещение между "сохранениями"
Для перемещение на другую фиксацию(коммит) испольщуется команда *git chrckout*. Для этого необходимо, как поканазано в прошлом пункте, в журнал изменений найти необходимый коммит и его хеш (номер), после чего в терманале с папкой-репозиторием надо написать *git checkout <хеш коммит>*. После выполнения этой команды ма попадаем в состояние **detached head**, в котором никакие следующие комииты сохраняться не бедут. Для выхода из этого состояния необходимо написать *git checkout master*.

## Журнал изменений
Для просмотра истории изменений используется комманда *git log*. Для этого в терменале с папкой-репозиторий необходимо написать *git log*.

## Ветки в git
Для того что бы создать ветку в Git необходимо воспользоваться командой *git branch <название ветки>*. Для того что бы проверить на какой ветке вы сейчас находитесь воспользуйтесь командой *git branch*, для переключения между ветками восопользуйтесь командой *git checkout <название ветки>*

#### Замечание
создаем ветку в терминале в папке-репозитории.

### Замечание по перемещению веток
Для того чтобы перемещаться между ветками, вы должны убедиться что такая ветка существует.

## Слияние веток и разрешение конфликтов
### Слияние веток
Для того чтобы слить разные ветки в главную воспользуйтесь командой *git merge<название ветки>* после того как ветки слили, можно удалить эту ветку, воспользуйтесь командой *git branch -d<название ветки>*.

### Разрешение конфликтов
Для того что бы разрешить конфликт можно восопльзоваться двумя опциями:
1. сделать это в автоматическом режиме, для этого необходимо при возниконовении конфликта выбрать мышкой нужную опцию, или принять все изменения, или выбрать только те что вам нужны.
2. Сделать вручную, для этого удалить знаки >>>>>, ===== и название веток.

После всех этих шагов необходимо выполнить следующие команды git add .\<название файла>, git commit -m "<Название коммита>".

## Удаление веток
Для удаления веток воспользуйте командой *git branch -d <назваение ветки>*
