Переменные:

clickhouse_version - версия кликхауса для разворачивания

clickhouse_packages - необходимые для установки пакеты компонентов

vector_version - версия вектора для разворачивания

vector_home - домашняя директория, куда класть внутренности вектора

Апдейт для занятия 3:

Добавлена переменная lighthouse_git — содержит адрес репы проекта лайтхаус.
Добавлены нормальные человеческие конфиги для пристойного функционирования всего хозяйства.

Плэйбук по шагам осуществляет установку вектора и кликхауса. Дописана секция, устанавливающая энжинкс и лайтхаус. Установка вектора идёт в несколько тасков, тегированных vector_dir (создание папки в opt), vector_unpack (распаковка) и vector_tempconfig (копирование темплейта конфига для вектора).
Установка лайтхауса и энжинкса также тегирована nginx_ready (установка nginx) и lighthouse_ready (установка lighthouse).
Установка кликхауса взята из любезно предоставленного исходного плэйбука.
