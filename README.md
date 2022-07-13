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
создаем 2 вм в облаке. на обеих вм выполняем следующие команды
sudo apt-get update
sudo apt install docker.io
sudo apt-get install -y apt-transport-https ca-certificates curl
sudo curl -fsSLo /usr/share/keyrings/kubernetes-archive-keyring.gpg https://packages.cloud.google.com/apt/doc/apt-key.gpg
echo "deb [signed-by=/usr/share/keyrings/kubernetes-archive-keyring.gpg] https://apt.kubernetes.io/ kubernetes-xenial main" | sudo tee /etc/apt/sources.list.d/kubernetes.list
sudo apt-get update
sudo apt-get install -y kubelet kubeadm kubectl
sudo apt-mark hold kubelet kubeadm kubectl
sudo kubeadm init --apiserver-cert-extra-sans=<external-master-ip> --apiserver-advertise-address=0.0.0.0 --control-plane-endpoint=<external-master-ip> --pod-network-cidr=10.244.0.0/16

После установки kubeadm будет пример команд по запуску кластера и добавления воркер ноды. команду по инит выполняем только на одной вм
на второй вм запускаем уже команду по добавлению воркера
