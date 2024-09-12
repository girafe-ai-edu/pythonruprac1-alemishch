[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/VqYIm5WW)
# PYTHON 2024
Рад всех приветствовать на курсе, посвященном программированию на языке Python!
Ниже вы найдете шпаргалку по работе с GitHub.

# Начало работы
1. Зарегистрируйтесь в Git, используя вашу корпоративную почту: [GitHub](https://github.com/)
2. Скачайте и установите Git Bash: [Git for PC](https://git-scm.com/downloads)
3. Залогиньтесь в Git Bash. Инструкция [здесь](https://kbroman.org/github_tutorial/pages/first_time.html)
4. Создайте на вашем ПК папку, в которой будете хранить файлы курса. Это ваш локальный репозиторий.
5. Скопируйте файлы из моего репозитория к себе в папку. Для этого нужно:

    a) Открыть коммандную строку Git Bash и перейти в вашу папку-локальный репозиторий. Используйте команду cd.

   b) После того, как вы убедились, что находитесь в нужной папке, склонируйте репозиторий к себе командой ниже:
   ```
   git clone <Ссылка на этот репозиторий>
   ```
   c) В вашей папке должны появиться папка с файлами . Один из файлов называется ".git". Если такой файл находится в папке, это означает, что папка является git-репозиторием.
   Далее все свои действия вы будете производить непосредственно с той папкой, в которой лежит данный файл.

6. В Web-клиенте GitHub перейдите в раздел "Репозитории" и создайте там новый репозиторий. Он должен быть "Public".
7. Для того, чтобы отправить файлы из вашей локальной папки на удаленный репозиторий, перейдите в папку  и воспользуйтесь командами ниже.

   [ссылка] - это ссылка на ваш git-репозиторий. Пример: https://github.com/girafe-ai-edu/edu_python_ru
   
   Просто перейдите в ваш репозиторий и скопируйте её из адресной строки. Или после https://github.com/ добавьте ваш ник и через косую черту название вашего репозитория. 
  ```
git add .
git commit -m "first commit"
git remote add pythonrep [ссылка]
git push -u pythonrep main
   ```

Вуаля, вы восхитительны, файлы появились на удаленном клиенте. Можете обновить страницу репозитория и лицезреть вашу работу. 

Этого достаточно для того, чтобы начать работу с GitHub. Ниже вы найдете полезные (или не очень) подсказки по вашей дальнейшей работе с Git.

# Рутинная работа
Чаще всего вы будете добавлять/изменять/удалять файлы в вашей локальной папке на ПК. После этого вам нужно отправить изменения на удаленный клиент GitHub.

Ваша основная задача сводится к командам, предложенным ранее. Ниже перечислены основные шаги для внесения изменений в репозиторий.
1. Добавьте необходимые вам файлы в список для отправки на сервер. Это делается командой 
  ```
git add .
   ```
Точка в конце говорит о том, что добавятся все измененные файлы. Можно добавить конкретный файл:
  ```
git add filename
   ```
2. После этого нужно подтвердить, что эти файлы готовы для отправки. Используем команду *git commit*. В кавычках указывается короткий текст сообщения о сути внесенных изменений. 
```
git commit -m "your text"
   ```
3. Отправляем изменения на сервер командой
  ```
git push -u pythonrep main
   ```
main - название ветки, изменения в которой вы хотите закоммитить. Это основная ветка. Вы попадаете в неё по умолчанию. 
В данном случае *pythonrep* - название, которое мы ранее закрепили на нашим удаленным репозиторием. Можно добавить несколько репозиториев с разными названиями командой 
  ```
git remote add repository_name [ссылка]
   ```
и коммитить в разные репозитории, указывая их название. 

После этого новые изменения появляются в Web-версии GitHub. 

Подробнее про работу с Git Bash можно посмотреть [Здесь](https://www.youtube.com/watch?v=a1RzYqD8kBU&t=1005s&ab_channel=%D0%90%D0%B9%D1%82%D0%B8%D1%88%D0%BD%D0%B8%D0%BA%F0%9F%91%A9%E2%80%8D%F0%9F%92%BB)
или почитать [Здесь](https://www.atlassian.com/git/tutorials/learn-git-with-bitbucket-cloud)

# Как сдавать ДЗ

Я отправляю вам ссылку вида *https://classroom.github.com/a/uI4Ehkwu* (пример)

Это ссылка на GitHub Classroom. Вы переходите по ней и добавляетесь в наш класс на GitHub. Автоматически на вашем аккаунте создастся репозиторий, в который нужно будет закоммитить файлы ДЗ до указанного дедлайна. 
Инструкция все та же:
1. Создаете локальную папку на ПК
2. В неё клонируете нужные файлы из вашего репозитория! 
3. Вносите изменения
4. Важно! Нужно добавить новый файлы.  Файлы добавляются командой
  ```
git remote add [имя файла или . для всех файлов]
   ```
5. Добавляете файлы и коммитите их на сервер в ваш репозиторий в NUSTMISIS
