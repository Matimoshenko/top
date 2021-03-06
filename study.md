# Инструкция по работе с git и удаленными репозиториями

## Что такое git?
> Git - это система управления версиями. Проект был создан Линусом Торвальдсом для управления разработкой ядра Linux, первая версия выпущена 7 апреля 2005 года. [Информация из Википедии](https://ru.wikipedia.org/wiki/Git)

*Git* - одна из реализаций распределенных систем контроля версий. *Git* на данный момент является самой популярной реализацией. Самой популярной реализацией *Git* является [GitHub](github.com) 

## Подготовка репозитория
Для того, чтобы создать репозиторий используется команда *git init*. Для этого необходимо написать в терминале в папке будущего репозитория *git init*

## Создание сохранений

### Добавление файла к коммиту
Для добавления файла к коммиту используется команда *git add*, пишется она следующим образом *git add <имя файла>* в папке с созданным рпозиторием.

### Создание коммита
Для создания нового "сохранения" используется команда *git commit*. Используется она следующим образом: в терминале с папкой-репозиторием пишется *git commit -m <сообщение к коммиту>*. Сообщение к коммиту писать обязательно.

## Журнал изменений

Для просмотра журнала изменений используется команда "git log". Для этого в терминале в папке с репозиторием достаточно написать *git log*.

## Перемещение между коммитами
Для перемещения между сохранениями используется команда *git checkout*. Для того, чтобы переместиться на указанный коммит в терминале в папке с репозиторием пишем *git checkout <номер коммита>*. **Номер коммита** берется из журнала изменений, о котором сказано выше. После перемещения на указанный коммит мы попадаем в состояние **detached head**. Чтобы вернуться к обычной работе, необходимо написать "git checkout master".

## Ветки в git
Для того, чтобы создать новую ветку, необходимо использовать команду *git branch*. Используется эта команда слудующим образом: *git branch <имя новой ветки>*. 
Также для перемещения между ветками используется команда *git checkout*. Для перехода к работе со следующей веткой необходимо ввести команду *git checkout <название ветки, на которую необходимо перейти>*.
Для вывода на экран списка всех веток, за изменениями в которых наблюдает git, необходимо ввести команду *git branch*, для этого просто набираем команду *git branch*.

Ветки в *Git* нужны, чтобы работать с чистовиком и черновиками. Для того, чтобы создать новую ветку используется команда branch: в терминале с репозиторием напишите *git branch <название ветки>*.

## Слияние веток и разрешение конфликтов
Для слияния веток используется команда *git merge*. Для этого с помощью команды *git chekout* выбирают ветку с которой будут проводить слияние. Затем пишут команду *git merge <имя ветки, которая будут сливать с выбранной ранее веткой>*.
При слиянии веток могут возникать конфликты, для их разрешения программа предлагает выбрать один из вариантов разрешения ситуации: выбрать первую ветку, выбрать вторую ветку, выбрать обе ветки сразу и внести изменения вручную.

Для слияния двух веток используется команда *git merge*. Для ее использования необходимо перейти в ту ветку, куда вы хотите сделать слияние. После чего в папке с репозиторием написать *git merge <название сливаемой ветки>*. Чаще всего слияние происходит автоматически, но возможны конфликты. В таком случае необходимо вручную получить желаемую версию файла и сделать коммит.

## Удаление веток
Для удаления веток используется команда *git branch -d <имя удаляемой ветки>*

Для удаления ветки используется комада *git branch -d*. Для этого необходимо в папке с репозиторием в терминале написать *git branch -d <название ветки>*. Удаляемая ветка обязательно должна быть слита.

## Получение удаленного репозитория

## Скачивание изменений удаленного репозитория

## Отправка изменений в удаленный репозиторий


