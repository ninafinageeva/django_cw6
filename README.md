Проект для создания и запуска рассылок
Для подключения базы данных необходимо указать ваши параметры в /config/settings(DATABASES) через ваш ".env" файл.

Сущности
Клиент сервиса:

контактный email;
Ф.И.О.;
описание.
Рассылка:

дата и время первой отправки рассылки;
периодичность(раз в день, раз в неделю, раз в месяц);
статус рассылки(создана, запущена, завершена);
название;
описание.
Сообщение для рассылки:

тема письма;
текст письма.
Попытка рассылки:

дата и время последней попытки;
статус попытки(успешно или нет);
ответ почтового сервиса если он был.

Сервис предназначен для массовой рассылки шаблонов сообщений адресатам.
Реализация произведена модулями Django в среде разработке Python 3.11. 
Шаблоны реализованы за счёт Bootstrap
Для работы с программой необходимо:

Установить зависимости командой "pip -r requirements.txt"
Переименовать файл .env_example в .env и внести необходимые данные
Создать аккаунт администратора коммандой python manage.py csu
Дополнительно
Данные для входа под аккаунтом администратора:
Логин: admin
Пароль: 1
Запустить сервер коммандой: python manage.py runserver
