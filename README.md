## [REST API](http://localhost:8080/doc)

## Концепция:

- Spring Modulith
    - [Spring Modulith: достигли ли мы зрелости модульности](https://habr.com/ru/post/701984/)
    - [Introducing Spring Modulith](https://spring.io/blog/2022/10/21/introducing-spring-modulith)
    - [Spring Modulith - Reference documentation](https://docs.spring.io/spring-modulith/docs/current-SNAPSHOT/reference/html/)

```
  url: jdbc:postgresql://localhost:5432/jira
  username: jira
  password: JiraRush
```

- Есть 2 общие таблицы, на которых не fk
    - _Reference_ - справочник. Связь делаем по _code_ (по id нельзя, тк id привязано к окружению-конкретной базе)
    - _UserBelong_ - привязка юзеров с типом (owner, lead, ...) к объекту (таска, проект, спринт, ...). FK вручную будем
      проверять

## Аналоги

- https://java-source.net/open-source/issue-trackers

## Тестирование

- https://habr.com/ru/articles/259055/

Список выполненных задач:
1.Remove "vk","yandex".
Знімок екрана 2024-06-06 203523

2.Extract sensitive information to a separate property file.
Знімок екрана 2024-06-06 203523

3.Write tests for all public methods of the ProfileRestController.
Знімок екрана 2024-06-07 144623

4.Refactor the method FileUtil#upload to a modern approach to working with the file system.
Знімок екрана 2024-06-07 144623

5.Add new functionality: adding tags to the task: REST API + implementation on the service.
Знімок екрана 2024-06-07 144623

6.Add localization in at least two languages for email templates and the index.html start page.
Знімок екрана 2024-06-09 124215

7.Write a Dockerfile for the primary server.
Знімок екрана 2024-06-12 184440

8.Write a docker-compose file to run the server container together with the database and nginx. For nginx, use the config file config/nginx.conf.
Знімок екрана 2024-06-12 184440

9.Rework the tests so that the in-memory database is used during the tests (H2)
...
