##           Framework: OSINT SAN. 
     Update black hawk 2.0

     Дата выхода версии 3.0 конец февраля, глобальное обновление будет платным.
     
     Зайдите в наш тг мы там анонсы бдущих обновлений выкладываем. Постоянно дорабатываем софт. Но на гит пока не выкладываем

Данный framework создан для сбора информации с открытых источников.
Но есть инструменты поиска и брутфорса которые использовать нужно, только с разрешения владельца ресурса, хочу вас предупредить что я не несу никакой ответственности за ваши действия при работе с фреймворком. В фреймворке используется большое количество API.

Наша официальная группа поддержки и обновлений: https://t.me/osint_san_framework

В бесплатной версии вам представленна demo версия " OSINT SAN 2.0 "

![alt tag](https://github.com/Bafomet666/screen/blob/main/55.png)​

В Framework используется много API нужно зарегистрироватся и получить всех API.

## Настройка всех API

     Название API и их путь.

     nomber api /OsintSan/plugins/api [http://apilayer.net/api]

     gmap api /OsintSan/plugins/api [https://developers.google.com/maps/documentation]

     ipstack api /OsintSan/plugins/api [https://ipstack.com/]

     shodan api /OsintSan/core/config and /OsintSan/api [https://www.shodan.io/]

     maildb api /OsintSan/plugins/maildb [Уже введен]

     hackertarget api /OsintSan/plugins/whois [Уже введен]

     whatcms /OsintSan/plugins/webosint/whatcms [https://whatcms.org/API]

     virus total /OsintSan/plugins/webosint/subdomain.py [Уже введен]

     macvendors /OsintSan/plugins/macaddress.py [https://macvendors.com/api]

     hunter /OsintSan/plugins/maildb.py hunter.io [https://hunter.io/api]

     ZoomEye Вход в API идет через авторизацию.

     Сensys [https://censys.io/api]  [же введен]


## Установка зависимостей.

Как только вы ввели свои API, вам нужно установить зависимости.
Установка легкая, вам потребуется python3 и установленный pip3.
После вам нужно в самой папке с фреймворком, открыть консоль и
прописать в ней, команду на установку зависимостей sudo pip3 install -r requerements.txt
после успешной установки, установите еще дополнительные зависимости, ниже.

         sudo apt install etherape
         pip3 install subprocess.run
         pip3 install wxPython
         sudo apt-get install adb
         sudo apt update
         sudo apt-get install android-tools-adb
         sudo apt install android-tools-adb android-tools-fastboot

## Переходим к авторизации.

Логин и пароль находятся в нашем телеграм канале, ссылка на него выше.


![alt tag](https://github.com/Bafomet666/screen/blob/main/Screenshot%20at%202021-01-16%2017-31-57.png)

После прохождения успешной авторизации, откроется меню с
инструментарием.

![alt tag](https://github.com/Bafomet666/screen/blob/main/update%202.0.png)

## Давайте перейдем к самим инструментам и их описанию.

## Функция 01.
Начнем с первого инструмента это проверка IP адреса в shodan and
census на утечки. Здесь все довольно просто, вбиваете адрес и
пользуете результат. Попробуем адрес google проверить, прописав
команду 8.8.8.8

![alt tag](https://github.com/Bafomet666/screen/blob/main/66.png)

После получения результата вас переместить в меню для
дальнейшего использования.

## Функция 02.
Работаем с доменным именем ( Это первая вкладка по доменному
имени )

![alt tag](https://github.com/Bafomet666/screen/blob/main/01.png)

Здесь все просто, выбираешь вариант и запускаешь, возможно
попросят указать дополнительные параметры. Полностью каждую
вкладку описывать смысла не вижу, те кто приобретает инструмент
уже знают что каждый пункт выполняет.

## Функция 03.
Базовый сбор информации о мобильном номере.
В будущем планируем подключить бота из telegram для получения
большей информации.

![alt tag](https://github.com/Bafomet666/screen/blob/main/02.png)

На стандартных API в месяц 50 запросов бесплатно.

## Функция 04.
Большая информативная карта dns сети.
После того как вы выбрали пункт 4, вам нужно вписать нужный вам
домен, примером я возьму яндекс. Следующем делом вам выведет
такое вот окно

![alt tag](https://github.com/Bafomet666/screen/blob/main/04.png)

можно идти в саму папку с фреймворком и смотреть карту

![alt tag](https://github.com/Bafomet666/screen/blob/main/05.png)

Карта обширная, в разрешении 2195x1285

## Функция 05.
Извлечение геолокации из фото.
Здесь вам нужно указать путь к фотo, для получения результата.
Пример пути : /home/bafomet/Downloads/Telegram
Desktop/IMG_9077421_731458.jpg

Очень большое количество данных выводит, запускать без root в
консоли.

## Функция 06.
Поиск по фото.
Вам нужно указать путь до картинки. После вас спросят хотите ли
вы открыть браузер, вы жмете “ y “ и открывается браузер.
После того как выполнится запрос вас опять переместит в меню.

![alt tag](https://github.com/Bafomet666/screen/blob/main/06.png)

Пока только google поиск, я хочу сделать чтобы поиск открывал
в 5 поисковых системах.

![alt tag](https://github.com/Bafomet666/screen/blob/main/08.png)

Ожидайте 5 функций поиска в 1 клик в “ V - 3.0 “

## Функция 07.
Проверка сервера либо IP адреса на HoneyPot ( ловушку для
хакеров )

![alt tag](https://github.com/Bafomet666/screen/blob/main/07.png)

Показывает все в процентах.

 # Функция 08. 
 Mac address info
 
     └──>  Выбери опцию :8
     └──> MAC адрес геолокация ( 08:00:69:02:01:FC ) :08:00:69:02:01:FC
     Компания:SILICON GRAPHICS INC.
     Адрес:2011 N. SHORELINE BLVD.,MOUNTAIN VIEW  CA  94039-7311,US
     Страна:US
     
# Функция 09. 
IP геолокация на картах.
Как по мне самые вкусное что я делал. IP геолокация GUI на картах.
При нажатии функции 9 вам выпадет вот такое окно.

![alt tag](https://github.com/Bafomet666/screen/blob/main/09.png)​

Далее вам нужно либо ввести IP адрес либо домен.
Вариант выберите обязательно.
Приведу пример:

![alt tag](https://github.com/Bafomet666/screen/blob/main/010.png)​

Эту систему буду внедрять в Big Bro 8.0
    
# Функция 10. 
Проверяем что качает через torrent в данный момент жертва.
Попутно узнаем её координаты.
 
![alt tag](https://github.com/Bafomet666/screen/blob/main/photo_2020-12-13_02-33-17.jpg)​

Если в данный момент, жертва ничего не загружает будет
выводиться окно:

![alt tag](https://github.com/Bafomet666/screen/blob/main/011.png)

# Функция 11.
OSINT Instagram.

![alt tag](https://github.com/Bafomet666/screen/blob/main/012.png)

# Функция 12.
Обычная проверка IP адреса на средства анонимности, я выгрузил с сети миллиардную базу IP адресов прокси серверов и vpn/ что бы проверять быстро на использования анонимайзеров. Из-за этого +300 мегабайт к фреимворку, позже сделаю через API что бы уменьшить вес.

![alt tag](https://github.com/Bafomet666/screen/blob/main/013.png)

# Функция 13.

Ищем адреса mail с сайтов. Используем API censys.

![alt tag](https://github.com/Bafomet666/screen/blob/main/014.png)

# Функция 14.
Подключение через ADB, точнее это оболочка для быстрого подключения. Обязательно установить все зависимости.

![alt tag](https://github.com/Bafomet666/screen/blob/main/015.png)

Пожалуйста не писать мне дурацкие вопросы, как вкл, почему не термукс не работает. 95% ошибок что мне задают, по поводу этого инструмента, это все гуглитcя первой страничкой в гугл, сначала изучите что такое adb android, потом пишите, если что то очень сложное, и не можете решить.

# Функция 15.
Все уже знают, и использовали мой Big Bro, если не премиум версию то free точно. Здесь стоит версия premiun на 40 сайтов.
Есть и бесплатная https://github.com/Bafomet666/Bigbro здесь и прочитаете подробное описание инструмента.

![alt tag](https://github.com/Bafomet666/screen/blob/main/6.5.png)

# Функция 16.
Массовый dump данных с Shodan. Работает через API, тот же поисковик только в консоли и анонимный.

![alt tag](https://github.com/Bafomet666/screen/blob/main/017.jpg)

# Функция 17.
Графический мониторинг твоей сети.

![alt tag](https://github.com/Bafomet666/screen/blob/main/99.png)

https://etherape.sourceforge.io/

https://ru.wikipedia.org/wiki/EtherApe

# Функция 18.
Сейчас эта функция нечего не загружает. Пока я не буду выкладывать dls либо другие обновления. Как минимум до конца января. Только глобальные. По причине не хочу заебывать вас мелкими обновами.

![alt tag](https://github.com/Bafomet666/screen/blob/main/016.png)

# Функция 19.
Инструкции внутри, будут доступны с 1 февраля. Сейчас они в альфа режиме.
Хотя я думаю зачем они вообще нужны когда вы можете здесь все прочитать, я наверное их уберу и добавлю какой нибуть инструмент хороший.

# Функция 20.
Список зависимостей я тоже уберу, и заменю его инструментом.

# Функция 21.
Журнал OSINT service. Огромный пак помощи по осинту.

![alt tag](https://github.com/Bafomet666/screen/blob/main/019.png)

# Функция 22.
Брутфорс instagram.
указываете логин и вперед. Если вдруг надо пароли сменить, в папке OSINT SAN есть документ password, удаляете все и вставляете свое.

# Функция 23.
VPN, Proxy, Tor. Страница с всеми отличными доступными анонимайзерами.

# Функция 24.
База данных паролей Bafomet +

Сейчас в базе 1.8 миллиарда паролей собрано. Все разбито по частями, что бы удобно было загружать. Пароли под различные задачи.

# Функция 25.
Поднимаем сайт Beff-XSS в сеть

Сначал вам нужно будет нажать 1. Это вариант с онлайном.
Потом вам выпадет инструкция по установке ngrok в положение ( start --all на 4 ссылки ) После вы запускаете ngrok в полном режиме и даете старт программе.

![alt tag](https://github.com/Bafomet666/screen/blob/main/020.png)

После вас попросят вписать ссылки, вписываем до http, https в таком формате:

     f19d35259оaff5.ngrok.io  всегда сначала по 80 порту
     
     f19d3c96533ff5.ngrok.io  потом по 3000 порту
     
А теперь установка стилей для сайта. Вам нужно перейти в папку "OSINT SAN" и скопировать все там из папки "Стили Beef" в директорию /var/www/html

Если вдруг у вас нет доступа к копированию стилей в beef html, Сделайте:
         
         sudo chmod 777 /var/www/htm


# Функция 26.
Наше большое сообщество OSINT СНГ. Здесь я собрал адреса всех ресурсов где есть полезная информация. Админов ресурсов знаю лично. Отличные парни.


# Функция 27.
Работа с доменом 2.0

![alt tag](https://github.com/Bafomet666/screen/blob/main/021.png)

# Функция 28.
Open Maltego, просто открывает мальтего.

![alt tag](https://github.com/Bafomet666/screen/blob/main/022.jpg)

# Функция 29.
Массовый dump данных с ZoomEye. Аналог shodan.
Вход через логин и пароль от самого сайта. Анонимный поиск с выбором с какой страницы дампить данные. Все данные сохраняются в папке с инструментом.

# Функция 30.
Деанонимизация хакера его же ссылкой, это обычный парсер, представим ситуацию, вам мамкин хакер скинул ссылку ngrok, что бы вы перешли и он узнал вашу геолокацию. Но вы возьмете эту ссылку и впишите в инструмент отслеживания и подождете, обычно он на себе ёё проверяет и деанонит себя.
Функция 30 направленна на то что бы автоматически воровать результат с его машины. Обратный деанон, Так-же можно отключить его ngrok, либо сломать, проверить с какого он железа работает. 

![alt tag](https://github.com/Bafomet666/screen/blob/main/024.png)

# Функция 31.
IP logger для профи, Firefox.
Вы можете создавать как ссылки логеры так и файлы. Практически любые.

# Функция 32.
Анонимный чат.(Ожидайте в след месяце)

# Функция 33.
dns whois сайтов.
![alt tag](https://github.com/Bafomet666/screen/blob/main/33.png)

# Функция 39. Секретная функция, запускать без root

# Функция 40. Лицензионное соглашение.
![alt tag](https://github.com/Bafomet666/screen/blob/main/sogl.png)


## Техническая поддержка.

![alt tag](https://github.com/Bafomet666/screen/blob/main/Screenshot%20at%202020-12-13%2002-02-20.png)​

Техническая поддержка осуществлется всем кто приобрел, либо поддержал разработчика, в течении трех месяцев, с момента приобретения.
При покупке все след обновления бесплатны.

Также фреимворк вы можете запускать как с рутом так и без. Часть функций требует рут а часть нет. Под каждым инструментом подписано.

Первый вариант это без рута полностью, в функциях подписано [N] значит, запускайте консоль без рута вообще  python3 osintsan.py.
Второй это уже с рутом, подпись [R], то есть запуск sudo python3 osintsan.py

Приятного использования.
