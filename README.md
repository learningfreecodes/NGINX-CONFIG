Анализ, комментирование конфигураций nginx

Чтобы применить новую конфигурацию 
```ssh
nginx -s reload
```
Если что-то не сработает как ожидалось нужно смотреть файлы `access.log` и `error.log` из каталога `/usr/local/nginx/logs` или `/var/log/nginx`

Чтобы остановить все процессы с ожиданием окончания всех обслуживающих запросов рабочими процессами 
```ssh
nginx -s quit
```
Тоже приведет к плавному завершению ```kill -s QUIT 1628```

Для просмотра всех запущенных процессов nginx ```ps -ax | grep nginx```