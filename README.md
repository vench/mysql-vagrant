# mysql-vagrant

mysql-vagrant is a quick way to run mysql locally for development without an ssh tunnel

### Start server

     $ vagrant up

### Connect to mysql:

- host: 33.33.33.1
- username: root
- password: root

### From sequel pro

<img src="sequel-pro.png"/>

### Инстуркция на русском

        Первый шаг запускаем в папке с кодом  vagrant up
        после успешной установки можно:
        1) Войти в shell виртуальной машины vagrant ssh и работать там с mysql
                mysql -uroot -p
        2) Работать с БД через прокинутый порт 3316
                mysql -uroot --host=33.33.33.1  --port=3316 -p
         
        Остановить машину vagrant suspend        
       

### Warning

For development use only, do not use in production.
Also, make sure your mysql port (3306) is not open on your computer for a local network or in general.

### License

MIT
