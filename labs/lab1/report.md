University: [ITMO University](https://itmo.ru/ru/)

Faculty: [FICT](https://fict.itmo.ru)

Course: [Introduction to distributed technologies](https://github.com/itmo-ict-faculty/introduction-to-distributed-technologies)

Year: 2022/2023

Group: K4110c

Author: Pochikalin Vladislav Olegovich

Lab: Lab1

Date of create: 10.09.2022

Date of finished: 10.09.2022

# Выполнение лабораторной работы

## Code trace

`minikube start` запуск кластера minikube

`minikube kubectl -- apply -f vault.yml` загрузка образа hashicorp vault и создание ресурса kubernetes

`minikube kubectl -- expose pod vault --type=NodePort --port=8200` создание объекта сервис, команда необходимая для того, чтобы получить доступ к поде извне

`minikube kubectl -- port-forward service/vault 8200:8200`  команда, которая прокидывает порт компьютера в контейнер 

`minikube stop`  остановка кластера

## Где взять токен? 

Токен можно найти, используя команду `minikube kubectl -- logs vault`

## Схема

![схема](https://github.com/blackberry22/2022_2023-introduction_to_distributed_technologies-k4111c-avdeeva_ml/blob/main/labs/lab1/schema.png)

## Расположение токена

![расположение токена](https://github.com/blackberry22/2022_2023-introduction_to_distributed_technologies-k4111c-avdeeva_ml/blob/main/labs/lab1/token.png)

## Результат работы

![результат работы](https://github.com/blackberry22/2022_2023-introduction_to_distributed_technologies-k4111c-avdeeva_ml/blob/main/labs/lab1/result.png)