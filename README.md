# Лабораторные по сетям

- Лабораторная №1

TCP сервер - запуск
```
go build server.go
./server [ip] [port] | [ip]
```
Если не указан port, то будет выбран стандартный 2156

Если не указан ip, то будет ожидаться ввод пользователя
 
TCP клиент - запуск
```
go build client.go
./client [ip] [port] [nik] | [ip] [nik]
```

Если не указан port, то будет выбран стандартный 2156

Если не указан ip, то будет ожидаться ввод пользователя

Если не указан nik, то будет ожидаться ввод пользователя

### Чат работает по следующему протоколу

Формат сообщения 
<timestamp> [nik] message
Размер отправляемого сообщения не ограничен.
Признак конца сообщения \n 