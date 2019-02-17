# devopsdeflope.ru

## Локальная работа

* `docker build -t deflope .`
* `decker run --rm --it --mount src=`pwd`,dst=/app,type=bind -p 4567:4567 deflope`

## Как добавить новый выпуск

- [ ] Добавить в `source/posts/<год>/` файл с описанием.
- [ ] Название файла с описанием в формате `<год>-<месяц>-<день>-<номер эпизода>.html.markdown`
- [ ] Добавить в `source/mp3/` запись выпуска. Название файла в формате: `deflope<номер выпуска>.mp3`. **Номер выпуска в названии mp3 и номер выпуска в файле с описанием должны совпадать!**
- [ ] Установить зависимости `bundle install`
- [ ] Собрать сайт `bundle exec middleman build`
- [ ] Запустить сайт и убедиться, что все выглядит правильно. `bundle exec middleman server`
- [ ] Задеплоить сайт `bundle exec middleman s3_sync`
- [ ] Загрузить запись выпуска на gdrive
