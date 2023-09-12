Установка и настройка Git [Инструкция](https://practicum.yandex.ru/catalog/free/"инструкция")
cd ~
mkdir project2
cd project2
git init
git status
touch readme.md
git status
git add readme.md (--all)(имя фаила, какой фаил)
git commit -m 'readme for look' (первый коммит)(сохранить)
git log (история комитов)
      github Repositories -> New -> u name 
      SSH ключ смотри [ТУТ](https://practicum.yandex.ru/catalog/free/"ТУТ")
git remote add origin git@github.com:petrovich566/project2.git
git remote -v (проверка) 
git push -u origin master (пуск)