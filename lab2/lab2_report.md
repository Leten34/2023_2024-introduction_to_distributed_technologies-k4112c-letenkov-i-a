University: [ITMO University](https://itmo.ru/ru/)  
Faculty: [FICT](https://fict.itmo.ru)  
Course: [Introduction to distributed technologies](https://github.com/itmo-ict-faculty/introduction-to-distributed-technologies)  
Year: 2023/2024  
Group: K4112c  
Author: Letenkov Ilya Alekseevich
Lab: Lab2  
Date of create: 17.11.2023  
Date of finished:  


1. Создаём файл деплоймента.  
![image](../lab2/img/1.png)


2. Создём манифест сервиса для доступа к подам.

![image](../lab2/img/2.png)


3. Деплоим выше описанные файлы.  
![image](../lab2/img/3.png)


4. Прокидываем порт. Приложение открывается в браузере.  
![image](../lab2/img/4.png)

5. Приложение работает. Значения переменных соответствуют тем, которые были переданы в коде. Также указано название пода и айпи - оно может меняться в завимости от того, в какой под идёт запрос. У нас две реплики, в браузере отображается информация одной из них.
![image](../lab2/img/5.png)


6. Проверены логи контейнеров. 
![image](../lab2/img/6.png)

Схема  
![image](../lab2/img/7.png)

Вывод: В результате выаолнения лаборатнорной работы в ранее созданном кластере Minikube было развернуто два пода с помощью deployment, после чего к ним был предоставлен доступ через сервис. Также в ходе работы были изучены принципы работы Depolyment и ReplicaSet, а также принципы распределения трафика между контейнерами.
