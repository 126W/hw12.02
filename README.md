# Домашнее задание к занятию "12.02 «Работа с данными (DDL/DML)»" - Евгений Шахов
---
### Задание 1

##### 1.1. Поднимите чистый инстанс MySQL версии 8.0+. Можно использовать локальный сервер или контейнер Docker.

##### 1.2. Создайте учётную запись sys_temp
> create user 'sys_temp'@'localhost' identified by '123';

##### 1.3. Выполните запрос на получение списка пользователей в базе данных. (скриншот)  
> ![image](https://user-images.githubusercontent.com/122415129/235264220-08f11fa2-18ae-4470-a65d-cc342b085c46.png)

##### 1.4. Дайте все права для пользователя sys_temp.
> grant all privileges on *.* to 'sys_temp'@'localhost';

##### 1.5. Выполните запрос на получение списка прав для пользователя sys_temp. (скриншот)  
> ![image](https://user-images.githubusercontent.com/122415129/235264282-69782d2d-bae8-4264-a12f-4e1e4ce4d7c4.png)

##### 1.6. Переподключитесь к базе данных от имени sys_temp.
> ![image](https://user-images.githubusercontent.com/122415129/235271853-9fecac86-7ec3-4b44-85d0-aabf3dec7465.png)
 
##### Для смены типа аутентификации с sha2 используйте запрос: ALTER USER 'sys_temp'@'localhost' IDENTIFIED WITH mysql_native_password BY 'password';  
#####  По ссылке https://downloads.mysql.com/docs/sakila-db.zip скачайте дамп базы данных.  
##### 1.7. Восстановите дамп в базу данных.

##### 1.8. При работе в IDE сформируйте ER-диаграмму получившейся базы данных. При работе в командной строке используйте команду для получения всех таблиц базы данных. (скриншот). Результатом работы должны быть скриншоты обозначенных заданий, а также простыня со всеми запросами.
> ![image](https://user-images.githubusercontent.com/122415129/235269788-fb961b97-1223-4f77-a8a5-58c623b93e16.png)

---
### Задание 2
##### Составьте таблицу, используя любой текстовый редактор или Excel, в которой должно быть два столбца: в первом должны быть названия таблиц восстановленной базы, во втором названия первичных ключей этих таблиц. Пример: (скриншот/текст)
> ![image](https://user-images.githubusercontent.com/122415129/235271221-65bde6ad-0d19-4b7c-98e7-200d89c57525.png)


---
