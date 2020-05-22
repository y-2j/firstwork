# firstwork
My first work with git

#### Команды для гита

git init

git add README.md

git commit -m "first commit"

git remote add origin https://github.com/stanruss/название.git

git push -u origin master

git log --oneline - посмотреть все коммиты.

git checkout . - восстановить все.

git checkout "код коммита" - вернуть до состояния этого коммита.

git checkout master - вернуться в ветку мастер.

Восстановить файлы на локальном компьютере:
git fetch --all

git reset --hard origin/master или git reset --hard origin/<название_ветки>

git add text.txt - Добавить файл в репозиторий

git rm text.txt - Удалить файл

git status - Текущее состояние репозитория (изменения, неразрешенные конфликты и тп)

git commit -a -m "Commit description" - Сделать коммит

git push origin - Замерджить все ветки локального репозитория на удаленный репозиторий 

git push origin master - Аналогично предыдущему, но делается пуш только ветки master

git push origin HEAD - Запушить текущую ветку, не вводя целиком ее название

git pull origin - Замерджить все ветки с удаленного репозитория

git pull origin master - Аналогично предыдущему, но накатывается только ветка master

git pull origin HEAD - Накатить текущую ветку, не вводя ее длинное имя

git fetch origin - Скачать все ветки с origin, но не мерджить их в локальный репозиторий

git fetch origin master - Аналогично предыдущему, но только для одной заданной ветки

git checkout -b some_branch origin/some_branch - Начать работать с веткой some_branch (уже существующей)

git branch some_branch - Создать новый бранч (ответвится от текущего)

git checkout some_branch - Переключиться на другую ветку (из тех, с которыми уже работаем)

git branch # звездочкой отмечена текущая ветвь - Получаем список веток, с которыми работаем

git branch -a # | grep something - Просмотреть все существующие ветви

git merge some_branch - Замерджить some_branch в текущую ветку

git branch -d some_branch - Удалить бранч (после мерджа)

git branch -D some_branch - Просто удалить бранч (тупиковая ветвь)

git show d8578edf8458ce06fbc5bb76a58c5ca4a58c5ca4 - Изменения, сделанные в заданном коммите

git push origin :branch-name - Удалить бранч из репозитория на сервере

git reset --hard d8578edf8458ce06fbc5bb76a58c5ca4a58c5ca4 - Откатиться к конкретному коммиту и удалить последующие (хэш смотрим в «git log»)

git push -f - залить на сервер измененные коммиты

git clean -f - Удаление untracked files



Работа с GIT для админов
Команды 

git status - состояние репа

git fetch - подтягивает все ветки с сервера

git fetch --all - подтягивает все вообще ветки

git checkout {название ветки} - переключение между ветками


git pull origin master - подтянуть все последние изменения

git checkout . - привести все отслеживаемые файлвы к состоянию до изменения

git clean -f -d - очистить от новых файлолв

git checkout -b {ID ветки} - создать ветку (номер задачи в джира например ASK-2934)

git commit -a -m"{ID задачи} {Название}" - закомитеть изменения (ид - обязательно писать номер задачи джира)

git push - отправить изменения на сервак или git push -u origin {ID вашей ветки} Отправка на сервер !Новой ветки

Пример ввода команд: 
git checkout master
git pull origin master
git checkout -b ASK-232323
{изменения в файлах}
git commit -a -m"ASK-232323 тут"
git status
git push -u origin {ID вашей ветки}

После push действия, через сайт gitlab создаем Мержреквест
Создаете новый где источник - ваша ветка, получатель alpha
