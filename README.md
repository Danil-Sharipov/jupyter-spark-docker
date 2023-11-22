# jupyter-spark-docker
## Запуск
```bash
touch env.env
echo "ADMIN={вашId}" >> env.env
echo "TOKEN={токенБота}" >>env.env
docker compose up -d
```
## Доступ к spark-master
При создании сессии в pyspark или запуска jar файла через spark-submit на мастер ноде --master spark://spark-master:7077