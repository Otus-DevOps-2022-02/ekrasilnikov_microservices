# ekrasilnikov_microservices

##ДЗ№12-13

Установка и знакомство с Docker. Запуск, управление, удаление образов и контейнеров. Сборка собственного образа на основе Dockerfile с дальнейшей загрузкой на docker hub. Запуск и проверка собственного образа в облаке и на локальной машине.

##ДЗ№14
Подготовка Dockerfile для сервисов приложения. Сборка docker образов на основе dockerfile, создание отдельной bridge сети для приложения. Создание и подклчючение volume для контейнера БД.

##ДЗ№15
Работа с сетями в Docker. Создание нескольких сетей типа Bridge, добавление сетей к контейнерам, для возможности разнесения сервисов приложения по разным подсетям. Установка и использование docker compose. Подготовка манифеста по сборке и запуску контейнера. Параметризация манифеста через env файл.

Для изменения префикса сущностей docker compose используется переменная окружения COMPOSE_PROJECT_NAME.

##ДЗ№16
Подготовка инсталяции GitLab. Подготовка репозитория, описание этапов пайплайна. Добавление раннера, тест пайплайна, добавление окружений

##ДЗ№17
Знакомство с прометеем. Подключение мониторинга контейнеров. Добавление прометея и node_exporter в docker-compose, развертывание в облачной инфраструктуре.

##ДЗ№18
Логирование docker контейнеров. Знакомство c Elastic Stack, fluentd. Работа с логами через kibana, Трейсинг через zipkin.

##ДЗ№19
Развертывание кластера Kubernetes. Подготовка двух виртуальных машин для кластера, одна как master, вторая как worker. Знакомство с kubeadm и kubectl. Подготовка и применение манифестов с Deployment. Установка и применение calico.

##ДЗ№20
Развертывание локального кластера kubernetes (minikube). Подготовка манифестов для развертывания в кластере kubernetes. Работа с kubectl, minikube.  Знакомство с service, namespace, selector. Запуск кластера kubernetes в Яндекс.Облаке с последующей раскаткой манифестов сервиса, и проверка работоспособности сервиса.

Скриншоты живут в ./kubernetes/screenshots

##ДЗ№21
Знакомство с ingress контроллером, установка и настройка в облачном кластере. Раскатка сервиса с использованием ingress + tls. Знакомство с NetworkPolicy, PersistentVolume, добавление PersistentVolume к сервису.

##ДЗ№22
Знвкомство с Helm. Применение манифестов через helm + tiller. Установка GitLab CI в кластере kubernetes, настройка CI и деплой сервиса.
