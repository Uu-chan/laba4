# Практическая работа №4, ZeroMQ
Реализована клиент-серверная программа с использованием ZeroMQ по паттерну PUB/SUB с использованием языка Python 3.6.1
При запуске сервера создается контекст и сокет его средствами с аргументом zmq.PUB, и биндится порт 11101, готовясь принимать подключения с любых адресов. Далее отсылается закодированное в юникод введеное сообщение пользователя.
Запустившийся клиент просит ввести (или скипнуть enter’ом для localhost) IPv4 или IPv6 адрес сервера, соответственно, создает контекст, сокет с zmq.SUB, соединяется с сервером, и ожидает в бесконечном цикле новых сообщений для печати.

