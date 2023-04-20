Программа для получения списка работодателей и их вакансий с сайта headhunter.ru и заполнения ими таблиц
в базе данных.

Код для создания таблиц в базе данных находится в файле create_db.sql внутри пакета fill_DB.

В пакете classes находится файл engine_HH.py, в нем написан код для парсинга необходимых данных по работодателям
и вакансиям.

В пакете fill_DB находится файл fill_database.py, в нем написан код для заполнения базы данных
данными по работодателям и вакансиям которые предлагают данные работодатели

В пакете db_manager находится файл db_manager.py, в нем написан код для работы с таблицами из базы данных
посредством SQL-запросов.

Для заполнения БД необходимо создать новую БД в программе PGAdmin после чего, создать таблицы в ней при помощи
кода из файла create_db.sql, после чего запустить main.py, после отработки программы таблицы будут заполнены
данными по работодателям и вакансиям, а также будут отработаны все методы написанные для работы с БД.

При повторном запуске (с тем же списком работодателей и вакансий) программа сообщит:
что данные работодатели уже существуют, то же относится и к вакансиям если они уже есть в базе.

Все классы и методы сопровождены докстрингами.