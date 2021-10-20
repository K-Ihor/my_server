# MY_SERVER(РКСОК) 1.0 

Рабоче-Крестьянский Стандарт Отправки Команд (РКСОК) 1.0 )))))

РКСОК версии 1.0 состоит из четырёх команд.

ОТДОВАЙ — для возврата данных
УДОЛИ — для удаления данных
ЗОПИШИ — для создания и обновления данных
АМОЖНА? — для получения разрешения обработки команды от специальных органов

Пример бращение у серверу:

1)  ОТДОВАЙ имя РКСОК/1.0
2)  ЗОПИШИ имя РКСОК/1.0
    телефон

Ответ сервера клиенту:

1)  НОРМАЛДЫКС РКСОК/1.0
    89012345678
2)  НОРМАЛДЫКС РКСОК/1.0

Первые три команды предназначены для работы с клиентами, 
которые могут запрашивать возврат данных, их удаление и сохранение.

А четвертая команда(АМОЖНА?) предназначена для общения сервера РКСОК с сервером дающий разрешение на выдачу или запись информации ))


Сервер запускаем ТАК ( "python3.9 async_server2.py") на 8000 порту.
Клиента для тестирование сервера ТАК ("python3.9 rksok_client.py 127.0.0.1 8000")
