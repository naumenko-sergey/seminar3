# **Инструкция по работе с Git**

![Эмблема GIT](git.png)

## Основная информация про Git

Git - это консольная утилита, для отслеживания и ведения истории изменения файлов, в вашем проекте. Чаще всего его используют для кода, но можно и для других файлов.
С помощью Git-a вы можете откатить свой проект до более старой версии, сравнивать, анализировать или сливать свои изменения в репозиторий.

## Инициализация репозитория

Для инициализации (создания) репозитория используется команда:

    git init

## Проверка сотояния репозитория

Чтобы проверить текущее состояние репозитория используется команда:

    git status

## Добавления в индекс

Для добавления изменений в индекс (это файл в котором содержаться изменения, подготовленные для добавления в коммит) используется команда

    git add

## Фиксация изменений

Для фиксации изменений внесенных в индекс используется команда:

    git commit

Коммит – это единица изменений в вашем проекте. Коммит хранит измененные файлы, имя автора коммита и время, в которое был сделан коммит. Кроме того, каждый коммит имеет уникальный идентификатор, который позволяет в любое время к нему откатиться.

## Статус текущего файла

Для того чтобы посмотреть статус текущего файла используется команда:

    git status

## Просмотр истории изменений

Для просмотра истории изменнений используется команда:

    git log


## Переключение между коммитами

Для перехода между добавленными коммитами используется команда:

    git checkout

## Просмотр изменений в файле

Для просмотра изменений в файле используется команда:

    git diff


## Ветвление

Почти каждая система контроля версий (СКВ) в какой-то форме поддерживает ветвление. Используя ветвление, Вы отклоняетесь от основной линии разработки и продолжаете работу независимо от неё, не вмешиваясь в основную линию. Во многих СКВ создание веток — это очень затратный процесс, часто требующий создания новой копии каталога с исходным кодом, что может занять много времени для большого проекта.

Некоторые люди, говоря о модели ветвления Git, называют ее «киллер-фича», что выгодно выделяет Git на фоне остальных СКВ. Что в ней такого особенного? Ветвление Git очень легковесно: операция создания ветки выполняется почти мгновенно, переключение между ветками туда-сюда, обычно, также быстро. В отличие от многих других СКВ, Git поощряет процесс работы, при котором ветвление и слияние выполняется часто, даже по несколько раз в день. Понимание и владение этой функциональностью дает вам уникальный и мощный инструмент, который может полностью изменить привычный процесс разработки.

### Создание новой ветки

Что же на самом деле происходит при создании ветки? Всего лишь создаётся новый указатель для дальнейшего перемещения. Допустим вы хотите создать новую ветку. Вы можете это сделать командой:

    git branch <branch name>

### Слияние веток

Слияние веток – это перенос изменений с одной ветки на другую. При этом слияние не затрагивает сливаемую ветку, то есть она остается в том же состоянии, что позволяет нам потом продолжить работу с ней. Теперь давайте перейдем к тому, как слияние реализовано в Git.

#### Команда слияние

Для того, чтобы влить ветку в текущую нужно использовать определенную команду:


    git merge <branch_name>

## Удаленные репозитории

Удаленные репозитории нужны
