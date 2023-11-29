University: [ITMO University](https://itmo.ru/ru/)  
Faculty: [FICT](https://fict.itmo.ru)  
Course: [Introduction to distributed technologies](https://github.com/itmo-ict-faculty/introduction-to-distributed-technologies)  
Year: 2023/2024  
Group: K4112c  
Author: Letenkov Ilya Alekseevich
Lab: Lab3  
Date of create: 26.11.2023  
Date of finished:  

1. Создём шаблон configMap с необходимыми переменными.  
![image](../lab3/img/1.png)

   
2. Создаём ReplicaSet, в который передаём указанные переменные.  
![image](../lab3/img/2.png)


3. Создаём tls секрет, в который прописываем созданные приватный и публичный ключ. 
![image](../lab3/img/3.png)
   
4. Создаём сервис для приложения.  
![image](../lab3/img/4.png)

5. Создаём ингресс. В него подтягиваем ключи из секрета, созданного ранее, а также указываем путь, по которому будет доступно наше приложение.  
![image](../lab3/img/5.png)

   
6. Деплоим всё вышеуказанное.  
![image](../lab3/img/6.png)

7. Далее достаточно запустить minikube addons enable ingress, а также minikube tunnel. 
![image](../lab3/img/7.png)

   
8. Переходим в браузер.
![image](../lab3/img/8.png)


9. Сертификат.  
![image](../lab3/img/9.png)

Схема  
![image](../lab3/img/10.png)

Вывод: В результате выполнения лабораторной работы был настроен веб-сайт, данные которого хранятся в кластере minikube, а доступ осуществляется по доменному имени. Были освоены основы работы с ingress, сертификатами и секретами.
