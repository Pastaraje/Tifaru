1. Переключаемся на master и обновляем ее - `git checkout master && git pull origin master`
2. Создаем ветку из master : `git checkout -b TIFA-000` (пример)
3. Делаем изменения в рамках поставленной задачи.
4. Коммитим изменения: `git commit -m "TIFA-000 fix something"`
5. Пушим наши изменения в ветку: `git push origin TIFA-000`
6. Создаем Merge Request в gitlub. Ждем апрува от ревьюера!!
7. Если есть конфликты идем в консоль.  
  7.1. Переключаемся на develop и обновляем его: `git checkout develop && git pull origin develop`  
  7.2. делаем мердж: `git merge --no-ff TIFA-000`
8. Резолвим конфликты и коммитим это с сообщением *"Fix merge conflict with TIFA-000"*
9. Делаем `git push origin develop`
10. После того как апрув получен окрываем консоль и переключаемся и обновляем ветку develop.
`git checkout develop && git pull origin develop`
11. Компилим стили: `npm run dev` и смотрим изменения `git status`

ЕСЛИ есть изменения в css файлах добавляем их и коммитим с сообщением *"Compile styles"*
Выливаем изменения в develop. Тестируем на дев сервере.
Если ни чего не сломанно - поздравляю Вы Молодец!!

>NOTE: если это хот фикс делаем его из последней ветки в которой велась разработка(запросить у девелопера)
