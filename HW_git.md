
# JSON
##### 1. Создать внешний репозиторий c названием JSON.

перейти на сайт `https://github.com` Залогиниться. Нажать кнопку `New`.

в поле Repository name ввести JSON, выбрать Public и Add a README file.

Нажать `Create repository`.

##### 2. Клонировать репозиторий JSON на локальный компьютер.

Нажать `Code`, выбрать HTTPS, скопировать ссылку на репозиторий,

на локальном компьютере  зайти в папку(в которой будет размещен репозиторий), запустить  gitbash 

`git clone https://github.com/zhuravskaya-anna/JSON.git` создать копию репозитория на локальном компьютере

`cd JSON`  (переходим в папку JSON (в конце адреса указано имя ветки  main )

##### 3. Внутри локального JSON создать файл “new.json”.

`touch new`.json файл создан

##### 4. Добавить файл под гит.
`git status` - проверить статус название файла new.json отображается красным (изменения в файле не отслеживаются) 

`git add .` -Эта команда добавит файл в раздел проиндексированных файлов Git (начинается отслеживание измений в файле)

`git status` - проверить статус Окрашенный зеленым цветом вывод «new file: new.json» сообщает о том, что файл  будет сохранен при выполнении следующего коммита   (изменения в файле отслеживаются)

##### 5. Закоммитить файл.
`git commit -m "add file new.json"` - создает снимок состояния (контрольную точку)  файла с комментарием add new.json

##### 6. Отправить файл на внешний GitHub репозиторий.

`git push`  выгружаем содержимое локального репозитория в удаленный репозиторий

##### 7. Отредактировать содержание файла “new.json” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате JSON.



`vim new.json`    воспользуемся встроенным редактором VIM открывается редактор
`i `  команда insert, вход в режим редактирования

        {
        	"person": {
        	"name":"Ganna",
        	"surname":"Zhuravskaja",
        	"age":28
        	},
        	"pets":[{
        		"number":1,
        		"kind_of_pet":"cat",
        		"name":"Salvador"},
        		{"number":2,
        		"kind_of_pet":"snail",
        		"name":"Lusinda"
        		}],
        
        	"desired_Salary":"500$"
        }

`Esc` выйти из режима редактирования

`:wq`  сохранить и выйти


##### 8. Отправить изменения на внешний репозиторий.
`git commit -am "add info  new.json"`  команда -am  аналогична запуску двух команд: git add для всех файлов, которые существовали в предыдущем коммите, и git commit с комментарием add info  new.json

`git push`  выгружаем содержимое локального репозитория в удаленный репозиторий

##### 9. Создать файл preferences.json

`cat > preferences.json` используем команду cat > для создания  и добавления информации в фойл непосредственно в консоли


##### 10. В файл preferences.json добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате JSON.

        {
        "preferences": {
        	"favorite_movie":" Men in Black",
        	"favorite_series":"Downton Abbey",
        	"favorite_food":"Pasta",
        	"favorite_season":"Spring",
        	"country_you_would_like_to_visit":"Brazil"
        		}
        }

`Ctrl + с ` сохранить и выйти из редактирования

##### 11. Создать файл sklls.json добавить информацию о скиллах которые будут изучены на курсе в формате JSON

`cat > skills.json`

            {
            "skills": [
              "software testing theory",
              "client-server architecture",
              "HTTP Server Request Methods",
              "HTTP server Response codes",
              "Structures of HTTP requests and responses",
              "JSON, XML",
              "API testing  - Postman",
              "Removing and reading logs from an external server",
              "Sniffing http web traffic through Charles and Fiddler",
              "Dev Tools of web browsers Google Chrome, FireFox",
              "VPN. (tool options)",
              "Mobile testing",
              "iOS, Android, guidelines",
              "Build iOS applications on Xcode",
              "Build Android applications on Android Studio",
              "ADB management of android devices",
              "Setting up proxy and vpn on iOS and Android",
              "Sniffing  of mobile traffic through Charles and Fiddler on iOS and Android",
              "Terminal Linux (copy, create, view, move files on servers without a graphical interface)",
              "Bash scripting, automation of routine tasks on the server",
              "Access to remote servers",
              "Basics of SQL (Create, Delete, Drop, Insert Into, Select, From, Where, Join)",
              "Postgres database (installation, configuration and use)",
              "Non-relational database Redis (installation, configuration and use)",
              "Load testing in Jmeter",
              "Scrum development methodology",
              "Python. Learning the basics. Building a client-server application"
              ]
            }


##### 12. Отправить сразу 2 файла на внешний репозиторий.

`git status` - проверить статус название файлов    отображается красным (изменения в файле не отслеживаются) 

`git add . ; git  commit -m "add 2 files preference skill" ; git push`  для выполнения нескольких команд подряд используется  символ `;`



##### 13. На веб интерфейсе создать файл bug_report.json.

Войти в репозиторий `JSON.` Нажать кнопку `Add file.`

Выбрать `Create new file`. В поле Name your file ввести `bug_report.json`.


##### 14. Сделать Commit changes (сохранить) изменения на веб интерфейсе.

Нажать кнопку `Commit new filе` в нижней части экрана


##### 15. На веб интерфейсе модифицировать файл bug_report.json, добавить баг репорт в формате JSON.

Открыть файл bug_report.json Выбрать  Edit this file. Ввести текст

            {
              "bug_report": {
                "id": 1,
                " Summary ": "Header->меню-> не верно назван элемент  Академия ",
                "Severity": "Minor",
                "Priority": "Medium",
                "Environment": "Windows 7 Professional 64-bit Google Chrome",
                "Description": "в заголовке сайта в меню  Block-4 не верно назван элемент указано  Главная  вместо  Академия ",
                "STR": " Запустить браузер. перейти  https: АДРЕС. в заголовке сайта изучить название  элементов меню. сравнить со спецификацией",
                "ER": "элемент   Академия  ",
                "AR": " элемент Главная  ",
                "Attachment" : "JPG"
              }
            }


##### 16. Сделать Commit changes (сохранить) изменения на веб интерфейсе.

Нажать кнопку `Commit new filе` в нижней части экрана

##### 17. Синхронизировать внешний и локальный репозиторий JSON

`git pull` используется для извлечения и загрузки содержимого из удаленного репозитория и немедленного обновления локального репозитория этим содержимым


********************
