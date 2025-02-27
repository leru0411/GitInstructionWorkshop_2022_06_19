# Инструкция по работе с git

## Что это и для чего нужна система контроля версий?

### Что такое система контроля версий?
Cистема контроля версий – это система, записывающая изменения
в файл или набор файлов в течение времени и позволяющая вернуться позже к определенной версии. Мы хотим гибко управлять некоторым набором файлом, откатываться до определенных версий в случае необходимости. Можно отменить те или иные изменения файла, откатить его удаление, посмотреть кто что-то поменял. Как правило системы контроля версий применяются для хранения исходного кода, но это необязательно. Они могут применяться для хранения файлов совершенно любого типа.
### Для чего нужна система контроля версий

## Установка git и VSCode на ваш ПК.

### Установка VSCode на ваш ПК.

1. Переходим на сайт code.visualstudio.com, секция Download
2. Здесь есть версия под Mac, Linux. Меня интересует Windows. Нажимаем и скачиваем себе на ПК
3. Программа скачана, запускаем инсталлятор и следуем инструкциям: принимаем, добавляем все галочки, далее, ждем пока программа установится на наш ПК.
4. Первое, что мы видим — это экран приветствия. Здесь есть пункт, с помощью которого мы можем импортировать все настройки, клавиши из уже установленных редакторов, например Vim, Sublime, Atom и другие.


### Установка git на ваш ПК

#### Первая настройка git

## Создание и базовая работа с локальным репозиторием.

### Что такое репозиторий и инструкция по созданию локальных репозиториев.

### Базовая работа с локальным репозиторием
git config --global user.name «Ваше имя английскими буквами» например: Konstantin

git config --global user.email ваша почта@example.com

git init – инициализация локального репозитория

git status – получить информацию от git о его текущем состоянии

git add – добавить файл или файлы к следующему коммиту

git commit -m “message” – создание коммита.

git log – вывод на экран истории всех коммитов с их хеш-кодами

git checkout – переход от одного коммита к другому

git checkout master – вернуться к актуальному состоянию и продолжить работу

команды для работы с ветвлением
git branch - вывод всех веток на экран

git branch <branch_name> - создание новой ветки

git checkout -b <branch_name> - создание и переключение на новую ветку

git checkout <branch_name> - переключение на новую ветку

git merge - слияние веток

git branch -d <branch_name> - удаление ветки

git log --graph - вывод истории комитов с визуализацией
## Ветки. Локальная работа с ветками в git.

### Что такое ветки и для чего они нужны при работе с системой контроля версий.

### Базовая работа с ветками в git.

## Работа с удаленными репозиториями.

### Что такое удаленный репозиторий и для чего он нужен


**Удаленный репозиторий** – это версии вашего проекта, сохраненные на удаленном сервере. Доступ к репозиторию на таком сервере может осуществляться по интернету или по локальной сети.

**Удаленный репозиторий** – полноценный репозиторий, ничем не отличающийся от локального. У удаленного репозитория есть собственные ветки, собственный указатель HEAD, своя история коммитов и так далее.

Для совместной удаленной работы.




### Базовая работа с удаленными репозиториями GitHub

## Совместная работа над проектом (fork, pull request)

### Как строится и для чего нужна совместная работа в системах контроля версий

### Инструкция по созданию pull request

## Книги и полезные ссылки по изучению git.

## Альтернативные системы контроля версий.
> GitLab

Еще до того, как GitHub попал в чужие руки, GitLab был довольно популярной альтернативой. Теперь я ожидаю, что это привлечет гораздо больше внимания. GitLab имеет открытый исходный код, и его базовая версия бесплатна. Есть также платные версии, они начинаются с 4 долларов за пользователя в месяц.

Это полный инструмент жизненного цикла DevOps с функциями планирования, тестирования, упаковки и выпуска. Он также имеет вики и функции отслеживания проблем. Вы можете развернуть GitLab внутри или в облаке.

> Gogs

Если безболезненная установка является вашей главной задачей, то для вас нет ничего лучше, чем Gogs. Он поставляется с готовыми к использованию двоичными файлами для Windows, Linux, Mac и Raspberry Pi, но вы также можете использовать Go, чтобы установить его на любую другую платформу, на которой работает Go.

Gogs легкий и быстрый, и хотя он не обладает всеми функциями больших дорогих костюмов, он поставляется с вики, отслеживанием ошибок, контролем версий и т. д.

> Trac

Trac — отличный выбор, если вы ищете минималистичную альтернативу GitHub. По сути, Trac — это расширенная вики-система и система отслеживания проблем для проектов разработки программного обеспечения. Для контроля версий он использует Git и Subversion, но может работать и с дюжиной других (например, Mercurial, Perforce и т. д.).

Благодаря хорошей функциональности отчетов, Trac является хорошим выбором, если вам необходимо регулярно и внимательно следить за ходом проектов.

> GitBucket

GitBucket — это клон GitHub, написанный на Scala. У него не так много функций, как у других приложений в списке. На самом деле его главное преимущество — это сходство с GitHub. Другими словами, если вы начинаете скучать по GitHub, вы всегда можете прибегнуть к GitBucket.

Его функции включают в себя просмотр репозитория, отслеживание проблем, запросы на извлечение и вики. Вы можете расширить его функциональность с помощью плагинов, но не ожидайте от них слишком многого.

> Mercurial

В отличие от другого программного обеспечения в этом списке, Mercurial полностью отличается от GitHub, поскольку он не использует сервер Git, хотя вы можете конвертировать ваши данные Mercurial в объекты Git. Mercurial — не единственная альтернатива GitHub, не относящаяся к git-серверам.
