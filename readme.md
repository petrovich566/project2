Установка и настройка Git [Инструкция](https://practicum.yandex.ru/catalog/free/"инструкция")<br>
cd~ <br>
**mkdir project2**<br>
**cd project2**<br>
git init<br>
git status<br>
**touch readme.md**<br>
git status<br>
git add readme.md (--all)(имя фаила, какой фаил)<br>
git commit -m 'readme for look' (первый коммит)(сохранить)<br>
git log (история комитов)<br>
      **github Repositories -> New -> U name**<br>
      **SSH ключ смотри [ТУТ](https://practicum.yandex.ru/catalog/free/"ТУТ")**<br>
git remote add origin `git@github.com:*name/name*.git` (привязка удаленного репозитория к локальному)<br> 
git remote -v (проверка)<br> 
git push -u origin master (пуск)<br>
       **Редактирование readme.md**<br>
git add readme.md<br>
git commit -m 'Редактирование'<br>
git push<br>
<br>
git log (показывает список коммитов с хеш, по хеш можно смотреть изменения)<br>
Author — имя автора и его электронная почта, Date — дата и время создания коммита.<br>
git log --oneline (сокрашенно, показывает только необходимое количество символов хеша)<br>
<br>
HEAD - служебный фаил, внутри HEAD — ссылка на служебный файл: refs/heads/master (или refs/heads/main в зависимости от названия ветки). Если заглянуть в этот файл, можно увидеть хеш последнего коммита.<br>
<br>
Статусы файлов в Git<br>
*Untracked* (англ. неотслеживаемый). Мы говорили, что новые файлы в Git-репозитории помечаются как untracked, то есть неотслеживаемые. Git «видит», что такой файл существует, но не следит за изменениями в нём. У untracked-файла нет предыдущих версий, зафиксированных в коммитах или через команду git add.<br>
*Staged* (англ.подготовленный). После выполнения команды git add файл попадает в staging area (от англ. stage — «сцена», «этап [процесса]» и area — «область»), то есть в список файлов, которые войдут в коммит. В этот момент файл находится в состоянии staged.<br>
*Tracked* (англ. отслеживаемый)
Состояние tracked — это противоположность untracked. Оно довольно широкое по смыслу: в него попадают файлы, которые уже были зафиксированы с помощью git commit, а также файлы, которые были добавлены в staging area командой git add. То есть все файлы, в которых Git так или иначе отслеживает изменения.<br>
*Modified* (англ. изменённый)
Состояние modified означает, что Git сравнил содержимое файла с последней сохранённой версией и нашёл отличия. Например, файл был закоммичен и после этого изменён.<br>
<br>
*Про staged и modified*
Команда git add добавляет в staging area только текущее содержимое файла. Если вы, например, сделаете git add file.txt, а затем измените file.txt, то новое содержимое файла не будет находиться в staging.
Git сообщит об этом с помощью статуса modified: файл изменён относительно той версии, которая уже в staging. Чтобы добавить в staging последнюю версию, нужно выполнить git add file.txt ещё раз.






