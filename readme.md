# Инструкци по работе с Git.
 
## Что такое Git?

## Подготовка репозитория

## Создание "сохранений"

## Перемещение между "сохранениями"
Для перемещение на другую фиксацию(коммит) испольщуется команда *git chrckout*. Для этого необходимо, как поканазано в прошлом пункте, в журнал изменений найти необходимый коммит и его хеш (номер), после чего в терманале с папкой-репозиторием надо написать *git checkout <хеш коммит>*. После выполнения этой команды ма попадаем в состояние **detached head**, в котором никакие следующие комииты сохраняться не бедут. Для выхода из этого состояния необходимо написать *git checkout master*.
## Журнал изменений

## Ветки в git

## Слияние веток и разрешение конфликтов

## Удаление веток