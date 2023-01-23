# Блог от Лизы

Блог на Django, серверная часть.

## Запуск

Для запуска блога у вас уже должен быть установлен Python 3.

- Скачайте код
- Скачайте данные для сайта [отсюда](https://dvmn.org/media/modules_dist/liza-backend-data.zip) и разархивируйте в директорию проекта.
- Установите зависимости командой `pip install -r requirements.txt`
- Запустите сервер командой `python3 manage.py runserver`

После этого переходите по ссылке [127.0.0.1:8000](http://127.0.0.1:8000), вы увидите главную страницу.

## Переменные окружения

Часть настроек проекта берётся из переменных окружения. Чтобы их определить, создайте файл `.env` рядом с `manage.py` и запишите туда данные в таком формате: `ПЕРЕМЕННАЯ=значение`.

**Для запуска проекта эти настройки не требуются**, значения уже проставлены по-умолчанию.

Доступны следущие переменные:
- `DEBUG` — дебаг-режим. Поставьте `True`, чтобы увидеть отладочную информацию в случае ошибки. Выключается значением `False`.
- `SECRET_KEY` — секретный ключ проекта. Например: `erofheronoirenfoernfx49389f43xf3984xf9384`.
- `ALLOWED_HOSTS` — см [документацию Django](https://docs.djangoproject.com/en/3.1/ref/settings/#allowed-hosts).
- `STATIC_URL` — по-умолчанию это `'/static/'`. [Что такое STATIC_URL](https://docs.djangoproject.com/en/3.0/ref/settings/#std:setting-STATIC_URL).
- `STATIC_ROOT` — по-умолчанию это `'None'`, т.е. текущая папка. [Что такое STATIC_ROOT](https://docs.djangoproject.com/en/3.0/ref/settings/#std:setting-STATIC_ROOT).
- `MEDIA_URL` — по-умолчанию это `'/media/'`. [Что такое MEDIA_URL](https://docs.djangoproject.com/en/3.0/ref/settings/#std:setting-MEDIA_URL).
- `MEDIA_ROOT` — по-умолчанию это `'media'`. [Что такое MEDIA_ROOT](https://docs.djangoproject.com/en/3.0/ref/settings/#std:setting-MEDIA_ROOT). 


## Страницы сайта

### Главная

Страница называется `index` и находится по адресу [http://127.0.0.1:8000](http://127.0.0.1:8000).

![Фото главной](https://github.com/atskayasatana/Images/blob/b7f70ccc8a9145d5dc5b4ddabea6ef574e29304e/2/main.png)


### Страница поста

На странице поста размещен текст поста, информация о посте(дата размещения, количество комментариев, количество лайков и прочее), а также комментарии к посту.

![Страница поста](https://github.com/atskayasatana/Images/blob/b7f70ccc8a9145d5dc5b4ddabea6ef574e29304e/2/post.png)


### Контакты

На странице с контактами указаны контакты владельцев сайта.

![Страница с контактами](https://github.com/atskayasatana/Images/blob/b7f70ccc8a9145d5dc5b4ddabea6ef574e29304e/2/contact.png)

## Цели проекта

Код написан в учебных целях — это урок в курсе по Python и веб-разработке на сайте [Devman](https://dvmn.org).
