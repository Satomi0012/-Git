# Что такое *Git*?

## Как установить *Git на Windows*

## Установка *Git на Linux*

## Первоначальная настройка и создание репозитория

## Подготовка репозитория

## Создание фиксаций

## Создание коммитов

## Выполнение коммита

## Добавление файла к коммиту

## Переключение между фиксацями

## Журнал изменений

## Ветки в Git

## Слияние веток и разрешение конфликтов

## Создание коммитов

## Удаление веток

Удаление веток не такой простой процесс, как может показаться. Можно случайно удалить несохраненные изменения в исходном коде, что приведет к нежелательным последствиям. Поэтому здесь нужно действовать осторожно. С операцией удаления над ветками справляется уже привычная команда git branch с параметром -d:

$ git branch -d <name of branch>

Для корректного удаления нужно помнить несколько правил, чтобы не получить ошибки:

    Нельзя удалить ветку, в которой вы находитесь. Git выкинет ошибку и не произведет удаление. Следовательно, нужно перейти на другую ветку.
    Git не позволит удалить ветку, у которой есть несохраненные изменения. Так мы избегаем ситуации, когда часть написанного кода будет безвозвратно утеряна. Если же мы уверены, что изменения в этой версии не нужны и их можно смело удалять, то вместо флага -d используем -D:

$ git branch -D <name of branch>

Соблюдая все условия, нам удастся удалить указанную ветвь.

## Что такое *Git push* и как его использовать

## Команда *Git remote add origin* для работы с удаленными репозиториями

## Команда *Git fetch* - чем отличается от *Git pull*

## Что такое *Git pull* и как его использовать