# Что такое *Git*?

Git — система управления версиями с распределенной архитектурой. В отличие от некогда популярных систем вроде CVS и Subversion (SVN), где полная история версий проекта доступна лишь в одном месте, в Git каждая рабочая копия кода сама по себе является репозиторием. Это позволяет всем разработчикам хранить историю изменений в полном объеме.

## Как установить *Git на Windows*

Переходим на официальный сайт Git, в раздел загрузок. Мы увидим несколько вариантов установки: разные разрядности, портативная версия и даже установка из исходников. Мы выберем Standalone-версию, для этого проще всего нажать ссылку Click here to download, она всегда ведет на самую актуальную версию. Запускаем скачанный файл.

## Установка *Git на Linux*

Также коротко покажем, как можно установить Git в различные дистрибутивы Linux. Как правило, самостоятельно скачивать ничего не нужно, достаточно воспользоваться встроенным в дистрибутив пакетным менеджером.

*Debian*

pt-get install git

*Ubuntu*

add-apt-repository ppa:git-core/ppa # apt update; apt install git

*Fedora 21*

yum install git

*Fedora 22+*

dnf install git

*Gentoo*

emerge --ask --verbose dev-vcs/git

*Arch Linux*

man -S git

*OpenSUSE*

ypper install git

*Mageia*

rpmi git

*FreeBSD*

pkg install git

*OpenBSD*

g_add git

*RHEL, CentOS, Oracle Linux и др.*

## Первоначальная настройка и создание репозитория

Перед началом работы с Git нужно указать свое имя и email, которые в дальнейшем будут записываться в историю изменений при каждом коммите. В будущем это позволит понять, кто именно внес те или иные изменения.

Откроем любое из приложений — Git Bash или Git CMD. Первое — это командная строка в стиле Linux, второе — командная строка в стиле Windows. Выбирайте то, что вам ближе. Мы выберем Git Bash и выполним две команды:

git config --global user.email "git-user@selectel.ru"
git config --global user.name "Selectel Git User"

Теперь Git полностью готов к работе. Давайте создадим репозиторий и зафиксируем в нем первое изменение (сделаем коммит). Для начала создадим каталог для будущего репозитория и сразу перейдем в него:

mkdir first-repo && cd first-repo

Создаем новый репозиторий в этом каталоге:

git init

Увидим ответ:

Initialized empty Git repository in C:/Users/git_user/first-repo/.git/.

Это означает, что в директории создан новый репозиторий. Далее создадим текстовый файл, назовем его README.md, и напишем в нем любой текст. Но сам по себе этот файл не попадет в следующий коммит. Мы должны проиндексировать изменения, то есть явно сказать Git-у, что этот файл нужно учитывать в следующем коммите:

git add README.md

Далее введем команду:

 git commit

Откроется текстовый редактор, который мы выбирали на этапе установки Git. Тут нам нужно ввести комментарий для коммита, то есть кратко описать изменение, которое мы сделали.

## Подготовка репозитория

## Создание фиксаций

## Создание коммитов

## Выполнение коммита

## Добавление файла к коммиту

## Переключение между фиксацями

## Журнал изменений

## Ветки в Git

## Слияние веток и разрешение конфликтов

## Удаление веток

## Что такое *Git push* и как его использовать

## Команда *Git remote add origin* для работы с удаленными репозиториями

## Команда *Git fetch* - чем отличается от *Git pull*

## Что такое *Git pull* и как его использовать