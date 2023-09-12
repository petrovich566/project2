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
git push