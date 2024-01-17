1. Используй памятку.
2. Если выдаёт ошибку - исправляй.
3. Если нет ключа - создай (путь создания не менять - Enter)
4. Пишем cat и пишем путь ssh
5. Создаём SSH key на Гитхаб через настройки и вставляем ключ, который сгенерировали.
6. Переходим в репозитирий - менять можно только index.js !!!
7. Переходим в репозиторий с index.js
8. Копируем SSH ссылку из зелёного Code
9. mkdir test - cd test - git clone {SSH}
10. ls - cd {название папки} - make install
11. code index.js (переходим в VSC) - размечаем все 5 пустышек
12. Настроить автосохр. либо вручную (Ctrl + S) - КРУЖОЧЕК
*Возможные ошибки в терминале* 
: make lint - make lint-fix - (Если нет error - то всё ок)
: export (перечисляем все 5 функций)
: node index.js (тестирует работоспособность функций)
: Перед каждым пушем - make lint-fix

13. Прописываем функции - выполняем задачи
14. git add,  git add -A,  git commit -m "task1",  git push
15. Можно посмотреть решение задач Максима по пробнику (Mattermost или Хекслет Ютуб канал)


Большинтсво функций можно найти в Mozilla / Веб-технологии для разработчиков / Math


# Как сделать коммит:

1. Отредактируйте файлы
2. Добавьте файлы в отслеживание командой **git add -A**
3. Сделайте коммит с сообщением командой **git commit -m "your_commit_message"**
4. Отправьте изменения в удалённый репозиторий командой **git push**
5. \*Если вы сделали изменения с другого ПК, либо кто-то другой что-то изменил в вашем репозитории, то перед началом работы следует воспользоваться командой **git pull**, чтобы избежать конфликтов

https://hexly.notion.site/d9289c18871c44508bc7c7f05a51d94f

1. ssh-keygen -t rsa
2. cat ~/.ssh/id_rsa.pub (enter enter enter)
3. Копируем SSH в Github и генерируем новый ключ через настройки
4. ssh -T git@github.com
5. // *1-4 нужны при работе с нового компа*
6. git clone {Зелёная SSH-ссылка}
7. ls - cd {название папки} 
8. cat Makefile
9. make install
10. code index.js
11. // *Автосохранение*
12. node index.js
13. make test
14. make lint
15. make lint-fix
16. // *Если остались ошибки - дело в файле*
17. make lint
18. git add -A
19. git commit -m «task»
20. git push

Главные команды это 

ls - посмотреть все файлы в директории   (Если добавить путь, то покажет содержимое указанной папки)
cd [название файла или путь] - войти в директорию
mkdir [название директории] - создать папку/директорию.
touch [название файла и его расширение] - создать файл.
mv [название файла] [путь до места назначения] - переместить файл.
code [название файла] - открыть файл в текстовом редакторе (VS code).
cat [название файла] - посмотреть содержимое файла(выведет содержимое в терминал.)
rm [название] - удаляет файл/папку.


Перед началом аттестации зайдите в свой аккаунт на компьютере. Для того, чтобы скачать репозиторий и делать коммиты вам нужно настроить SSH ключ. Как это сделать:

1. Проверьте, что у вас есть SSH-ключ введя в терминале команду: `ssh -T git@github.com`.
2. Если доступ закрыт, вам нужно будет сгенерировать SSH-ключ, прочитать его и установить в настройках GitHub:
    - `ssh-keygen` - эта команда генерирует ssh ключ. Каждый раз при вопросе нажимайте ентер.
    - `cat ~/.ssh/id_rsa.pub` - эта команда читает содержимое ssh ключа.
    - Войдите в свой профиль на гитхабе. Зайдите в настройки профиля (клик по иконке профиля справа вверху, настройки), перейдите в раздел "SSH-ключи", нажмите New ssh key. Ведите имя ключа в поле сверху, а все прочитанное содержимое нового ключа в поле ниже. Затем нажмите кнопку добавить.
3. Снова проверьте команду `ssh -T git@github.com`. В случае успеха вы должны увидеть приветствие по имени аккаунта.
4. Склонируйте репозиторий по SSH(!), попробуйте сделать коммит и запушить. Гит попросит вас установить глобальное имя пользователя и почту. Воспользуйтесь командами, которые подсказывает терминал и напишите глобальное имя, которое является вашим никнеймом на гитхабе и почту без кавычек. Снова попробуйте запушить. Если пуш прошел, значит вы успешно настроили окружение.
