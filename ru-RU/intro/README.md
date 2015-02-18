---
root: true
name: Вступление
sort: 0
---

# Что такое Gogs?

Gogs(Go Git Service) — удобная служба для собственного Git-репозитория, написанная на языке Go.

## Цели

Целью данного проекта является создать самый простой, быстрый и наиболее безболезненный способ настроить самостоятельно принимала Git обслуживание. С помощью языка Go, это может быть реализовано в независимом бинарном дистрибутиве для **всех платформы **, что поддерживает Go, в том числе Linux, Mac OS X, и Windows.

## Системные требования

- Веб-фреймворк: [github.com/Unknwon/macaron](https://github.com/Unknwon/macaron)
- UI-фреймворк: [GitHub Octicons](https://octicons.github.com/) + [Font Awesome](http://fontawesome.io/)
- ORM: [github.com/go-xorm/xorm](https://github.com/go-xorm/xorm)
- Подключение к БД: [github.com/go-sql-driver/mysql](https://github.com/go-sql-driver/mysql) или [github.com/lib/pq](https://github.com/lib/pq) или [github.com/mattn/go-sqlite3](https://github.com/mattn/go-sqlite3)

## Структура директорий

```
cmd/								// команды
conf/								// конфигурация
  |__ content/						// глобальный контент
  |__ gitignore/		
  |__ license/				
  |__ locale/						// i18n локали
etc/
models/								// бизнес логика
modules/							// вспомогательные модули
  |__ auth/							// авторизация
  |__ avatar/						// сервис работы с gravatar
  |__ base/							// общие функции и типы
  |__ captcha/							
  |__ cron/						
  |__ git/							// git shell
  |__ httplib/						// работа с HTTP
  |__ log/					 
  |__ mailer/						
  |__ middleware/						
  |__ process/						// менеджер процессов
  |__ setting/						// настройки приложения
  |__ social/						// OAuth2
  |__ ssh/							// SSH сервер(прототип)
  |__ uuid/							
public/								// статика
routers/							// контроллеры
scripts/							// вспомогательные скрипты
templates/								
```
