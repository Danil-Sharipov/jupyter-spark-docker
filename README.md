# jupyter-spark-docker
## Запуск
```bash
touch env.env
echo "ADMIN={вашId}" >> env.env
echo "TOKEN={токенБота}" >>env.env
docker compose up -d
```
Структура проекта
.
├── README.md
├── alertmanager
│   ├── config.yml
│   └── data
├── data
├── docker-compose.yml
├── env.env
├── grafana
│   ├── alerting
│   │   └── 1
│   │       └── __default__.tmpl
│   ├── dashboards
│   │   ├── dashboard.yml
│   │   ├── docker_containers.json
│   │   ├── docker_host.json
│   │   ├── monitor_services.json
│   │   └── nginx_container.json
│   └── provisioning
├── notebook
├── prometheus
│   ├── alert.rules
│   └── prometheus.yml
└── worker_data
## Доступ к spark-master
При создании сессии в pyspark или запуска jar файла через spark-submit на мастер ноде --master spark://spark-master:7077