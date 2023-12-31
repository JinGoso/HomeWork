# Git для новичков

## Что такое *Git* и зачем он нужен? new

**Git** - это консольная утилита, для отслеживания и ведения истории изменения файлов, в вашем проекте. Чаще всего его используют для кода, но можно и для других файлов. 

С помощью **Git**-a вы можете откатить свой проект до более старой версии, сравнивать, анализировать или сливать свои изменения в репозиторий.

*Репозиторием называют хранилище вашего кода и историю его изменений. Git работает локально и все ваши репозитории хранятся в определенных папках на жестком диске.* 

Так же ваши репозитории можно хранить и в интернете. Обычно для этого используют три сервиса :
 - GitHub
 - Bitbucket
 - GitLab

 Каждая точка сохранения вашего проекта носит название коммит (commit). У каждого commit-a есть hash (уникальный id) и комментарий. Из таких commit-ов собирается ветка. Ветка - это история изменений. У каждой ветки есть свое название. Репозиторий может содержать в себе несколько веток, которые создаются из других веток или вливаются в них.

## Как работает

Если посмотреть на картинку, то становиться чуть проще с пониманием. Каждый кружок, это commit. Стрелочки показывают направление, из какого commit сделан следующий. Например C3 сделан из С2 и т. д. Все эти commit находятся в ветке под названием main. Это основная ветка, чаще всего ее называют master . Прямоугольник main* показывает в каком commit мы сейчас находимся, проще говоря указатель.

![]()

В итоге получается очень простой граф, состоящий из одной ветки (main) и четырех commit. Все это может превратиться в более сложный граф, состоящий из нескольких веток, которые сливаются в одну.

![]()

## Основные команды

Для работы очень пригодятся следующие команды: 

 - git init - создание репозитория
 - git help - справка по всем командам
 - git add file_name - добавление файла в репозиторий
 - git status - просмотр статуса
 - git commit -m "" - добавляем новый файл с комментарием
 - git branch - добавление ветки
 - git checkout -переход к ветке
 - git merge - слияние ветвей
 - git log - просмотр истории проекта
 
## Wiki-history 

Git (произносится «гит»[7]) — распределённая система управления версиями. Проект был создан Линусом Торвальдсом для управления разработкой ядра Linux, первая версия выпущена 7 апреля 2005 года. На сегодняшний день его поддерживает Джунио Хамано.

Среди проектов, использующих Git — ядро Linux, Swift, Android, Drupal, Cairo, GNU Core Utilities, Mesa, Wine, Chromium, Compiz Fusion, FlightGear, jQuery, PHP, NASM, MediaWiki, DokuWiki, Qt, ряд дистрибутивов Linux.

Разработка ядра Linux велась на проприетарной системе BitKeeper[8], которую автор — Ларри Маквой, сам разработчик Linux — предоставил проекту по бесплатной лицензии. Разработчики, высококлассные программисты, написали несколько утилит, и для одной Эндрю Триджелл произвёл реверс-инжиниринг формата передачи данных BitKeeper. В ответ Маквой обвинил разработчиков в нарушении соглашения и отозвал лицензию, и Торвальдс взялся за новую систему: ни одна из открытых систем не позволяла тысячам программистов кооперировать свои усилия (тот же конфликт привёл к написанию Mercurial). Идеология была проста: взять подход CVS и перевернуть с ног на голову[9], и заодно добавить надёжности.

"*I'm an egotistical bastard, so I name all my projects after myself. First Linux, now git.*" - **Linus Benedict Torvalds**

# Как отправить *pull request*

1. Делаем fork интересуещего репозитория.
2. Делаем git clone для нашей версии этого репозитория.
3. Создаем ветку для изменений.
4. Производим изменения только в этой ветви.
5. Отправляем изменения на свой аккаунт (push)
6. В окне на GitHub появится возможеность отправить pull request.
