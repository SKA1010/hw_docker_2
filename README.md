# Домашнее задание к занятию «Docker. Часть 2»

### Задание 1

**Напишите ответ в свободной форме, не больше одного абзаца текста.**

Установите Docker Compose и опишите, для чего он нужен и как может улучшить вашу жизнь.

**Решение 1**

Docker Compose предназначен для развёртывания нескольких зависимых контейнеров. С его помощью этого плагина удобно разворачивать многоконтейнерные приложения.

---

### Задание 2 

**Выполните действия и приложите текст конфига на этом этапе.** 

Создайте файл docker-compose.yml и внесите туда первичные настройки: 

 * version;
 * services;
 * networks.

При выполнении задания используйте подсеть 172.22.0.0.
Ваша подсеть должна называться: <ваши фамилия и инициалы>-my-netology-hw.

**Решение 2**

Файл создан

https://github.com/SKA1010/hw_docker_2/blob/main/docker_1.yaml

---

### Задание 3 

**Выполните действия и приложите текст конфига текущего сервиса:** 

1. Установите PostgreSQL с именем контейнера <ваши фамилия и инициалы>-netology-db. 
2. Предсоздайте БД <ваши фамилия и инициалы>-db.
3. Задайте пароль пользователя postgres, как <ваши фамилия и инициалы>12!3!!
4. Пример названия контейнера: ivanovii-netology-db.
5. Назначьте для данного контейнера статический IP из подсети 172.22.0.0/24.

**Решение 3**

Конфиг установки контейнера с Postgresql

https://github.com/SKA1010/hw_docker_2/blob/main/docker_2.yaml

---

### Задание 4 

**Выполните действия:**

1. Установите pgAdmin с именем контейнера <ваши фамилия и инициалы>-pgadmin. 
2. Задайте логин администратора pgAdmin <ваши фамилия и инициалы>@ilove-netology.com и пароль на выбор.
3. Назначьте для данного контейнера статический IP из подсети 172.22.0.0/24.
4. Прокиньте на 80 порт контейнера порт 61231.

В качестве решения приложите:

* текст конфига текущего сервиса;
* скриншот админки pgAdmin.

Сервис установлен

https://github.com/SKA1010/hw_docker_2/blob/main/docker_3.yaml

![image](https://github.com/SKA1010/hw_docker_2/assets/125235217/5a431321-73cf-49c3-b886-956acf6ff3b6)

---

### Задание 5 

**Выполните действия и приложите текст конфига текущего сервиса:** 

1. Установите Zabbix Server с именем контейнера <ваши фамилия и инициалы>-zabbix-netology. 
2. Настройте его подключение к вашему СУБД.
3. Назначьте для данного контейнера статический IP из подсети 172.22.0.0/24.

**Решение 5**

Конфиг для Zabbix

https://github.com/SKA1010/hw_docker_2/blob/main/docker_4.yaml

---

### Задание 6

**Выполните действия и приложите текст конфига текущего сервиса:** 

1. Установите Zabbix Frontend с именем контейнера <ваши фамилия и инициалы>-netology-zabbix-frontend. 
2. Настройте его подключение к вашему СУБД.
3. Назначьте для данного контейнера статический IP из подсети 172.22.0.0/24.

**Решение 6**

Фронтэнд для Zabbix установлен

https://github.com/SKA1010/hw_docker_2/blob/main/docker_5.yaml

---

### Задание 7 

**Выполните действия.**

Настройте линки, чтобы контейнеры запускались только в момент, когда запущены контейнеры, от которых они зависят.

В качестве решения приложите:

* текст конфига **целиком**;
* скриншот команды docker ps;
* скриншот авторизации в админке Zabbix.

**Решение 7**

Сервис запущен

![image](https://github.com/SKA1010/hw_docker_2/assets/125235217/b4de3a3e-84b6-4116-98cc-1e5e11511c2c)


Итоговый конфиг

https://github.com/SKA1010/hw_docker_2/blob/main/docker-compose.yaml

---

### Задание 8 

**Выполните действия:** 

1. Убейте все контейнеры и потом удалите их.
1. Приложите скриншот консоли с проделанными действиями.

---

**Решение 8**

Контейнеры удалены
