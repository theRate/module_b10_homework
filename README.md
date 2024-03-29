# Skillfactory
## B10.6. Контрольный проект

### Ваше задание - написать telegram-бота, в котором будет реализован следующий функционал:

1. Бот возвращает цену на определённое количество валюты (евро, доллар или рубль).
2. При написании бота необходимо использовать библиотеку **_pytelegrambotapi_**.
3. Человек должен отправить сообщение боту в виде **<имя валюты цену которой он хочет узнать> <имя валюты в которой надо узнать цену первой валюты> <количество первой валюты>**.
4. При вводе команды **_/start_** или **_/help_** пользователю выводятся инструкции по применению бота.
5. При вводе команды **_/values_** должна выводиться информация о всех доступных валютах в читаемом виде.
6. Для взятия курса валют необходимо использовать любое удобное _API_ и отправлять к нему запросы с помощью библиотеки _Requests_.
7. Для парсинга полученных ответов использовать библиотеку _JSON_.
8. При ошибке пользователя (например, введена неправильная или несуществующая валюта или неправильно введено число) вызывать собственно написанное исключение **_APIException_** с текстом пояснения ошибки.
9. Текст любой ошибки с указанием типа ошибки должен отправляться пользователю в сообщения.
10. Для отправки запросов к **_API_** описать класс со статическим методом **get_price()**, который принимает три аргумента: имя валюты, цену на которую надо узнать, — **_base_**, имя валюты, цену в которой надо узнать, — **_quote_**, количество переводимой валюты — **_amount_** и возвращает нужную сумму в валюте.
11. Токен _telegram_-бота хранить в специальном конфиге (можно использовать _.py_ файл).
12. Все классы спрятать в файле **_extensions.py_**.
