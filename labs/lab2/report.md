University: [ITMO University](https://itmo.ru/ru/)

Faculty: [FICT](https://fict.itmo.ru)

Course: [Introduction to distributed technologies](https://github.com/itmo-ict-faculty/introduction-to-distributed-technologies)

Year: 2022/2023

Group: K4110c

Author: Pochikalin Vladislav Olegovich

Lab: Lab2

Date of create: 20.09.2022

Date of finished: 20.09.2022

# Выполнение лабораторной работы

## Code trace


Запустим кластер и создадим новый deployment
```bash
minikube start  
minikube kubectl -- apply -f lab2.yaml 
```
Результат можно проверить, перейдя по ip ноды и порту 30200

![result1](https://github.com/Whatislove118/2022_2023-introduction_to_distributed_technologies-k4110c-pochikalin_vo/blob/master/labs/lab2/node.png)

Обновим переменные и применим изменения.
```bash
minikube kubectl -- apply -f lab2.yaml 
```
Проверим, что обновления были применены и убедимся, что значения переменных поменялись

![result2](https://github.com/Whatislove118/2022_2023-introduction_to_distributed_technologies-k4110c-pochikalin_vo/blob/master/labs/lab2/after_apply.png)

Выведем логи

```bash
minikube kubectl -- logs lab2-deployment74645dd58c-p4s7h
```

![logs](https://github.com/Whatislove118/2022_2023-introduction_to_distributed_technologies-k4110c-pochikalin_vo/blob/master/labs/lab2/logs.png)


## Схема 

![scheme](https://github.com/Whatislove118/2022_2023-introduction_to_distributed_technologies-k4110c-pochikalin_vo/blob/master/labs/lab2/schema.png)