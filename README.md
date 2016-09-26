# activecollab_ru_RU
Русская локализация Activecollab 5.x

Кладем файлы:
ru_RU.UTF-8-backend.php - кладем в папку activecollab/5.9.13/localization/
application.ru_RU.UTF-8.js - кладем в папку activecollab/5.9.13/frontend/javascript/

Для тех, кто хочет исправить вывод дат на русском (сейчас выводятся на английском)
Необходимо поместить файл libraries.js в папку activecollab/5.9.13/frontend/javascript/

Если ещё не добавляли запись в базу данных колобка, необходимо это сделать, в таблицу "languages". Если добавляли, пропустить данный пункт.

Можно выполнить запрос через phpMyAdmin:

INSERT INTO `languages`(`name`, `locale`, `decimal_separator`, `thousands_separator`, `is_rtl`, `is_community_translation`, `is_default`, `updated_on`) VALUES ("Русский", "ru_RU.UTF-8", ".", ",", "0", "1", "0", UTC_TIMESTAMP())
