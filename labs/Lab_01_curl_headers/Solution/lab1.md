Отчёт к лабораторной работе №1
"HTTP HTTPS и их параметры"

GET запрос

$ curl -I https://aliexpress.ru

Получил код:

```git
 % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0   239    0     0    0     0      0      0 --:--:--  0:00:02 --:--:--     0HTTP/1.1 301 Moved Permanently
Server: Tengine
Date: Tue, 17 Oct 2023 11:31:30 GMT
Content-Type: text/html
Content-Length: 239
Connection: keep-alive
Location: https://aliexpress.ru/
EagleEye-TraceId: 211675d116975422902338055e1e5a
Timing-Allow-Origin: *
``````

Описание к коду:
```git
$ curl -I aliexpress.ru - Получение заголовков HTTP (ключ -I) с сайта Алиэкспресс

% Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--  
  0HTTP/1.1 301 Moved Permanently - запрашиваемый ресурс на постоянной основе переехал на новый адрес. Тогда новый путь к ресурсу указывается сервером в заголовке Location ответа
Date - дата нашего запроса
Content-Type: text/html; charset=UTF-8 - формат, в котором будут передаваться данные в теле запроса или ответа (текстовый формат с заголовком HTML и кодировкой UTF-8)
Content-Length - количество байт данных в теле запроса или ответа
Connection: keep-alive - постоянное http соединение
Location: https://aliexpress.ru/ - ссылка на сайт, куда мы переходим
EagleEye-TraceId - идентификатор для нескольких запросов
iming-Allow-Origin - стандарт безопасности
`````

