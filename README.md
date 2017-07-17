# SSHFileManager

Файл-менеджер для файлопомойки без дисплея, например Raspbery Pi. Позволяет смонтировать/размонтировать подключенную флешку. Умеет копировать файлы в фоновом режиме, не блокируя текущую сессию и позволяет ее разрывать, причем виден статус копирования.

Не требует никаких серверных демонов, все работает через ssh.

# Внимание!

Для корректной работы надо (п.1-2 для любителей урезать buildroot до минимума):

1.	lsblk -r
2.	nohup, cp, mv, df, mount, umount
3.	Папка /tmp/, желательно замонтированная на tmpfs
4.	Рутовый аккаунт, или тот, которому можно писать в /tmp/ и монтировать диски

Проверено на последнем дебиане и на последней сусе - работает отлично.

Это учебный проект, потому замечания насчет велосипедов и косяков в коде очень приветствуются.

# Что не доделано

1.	Закачка на сервер с устройства и наоборот. Будет позже, ибо мне оно пока не надо.
2.	Форматирование и разбиение дисков (опасная опция, нужна ли она вообще?)
3.	Работа с файлами (открыть, удалить, переименовать, свойства)
4.	Функционал быстрой отправки файлов на сервер из других программ (кнопка "Поделиться...")

# Скриншоты

<img src="https://github.com/konachan700/SSHFileManager/raw/master/img/Screenshot_1500297582.png" width="180px" align="left">
<img src="https://github.com/konachan700/SSHFileManager/raw/master/img/Screenshot_1500297591.png" width="180px" align="left">
<img src="https://github.com/konachan700/SSHFileManager/raw/master/img/Screenshot_1500297660.png" width="180px" align="left">
<img src="https://github.com/konachan700/SSHFileManager/raw/master/img/Screenshot_1500297669.png" width="180px" align="left">
<img src="https://github.com/konachan700/SSHFileManager/raw/master/img/Screenshot_1500297691.png" width="180px" align="left">

