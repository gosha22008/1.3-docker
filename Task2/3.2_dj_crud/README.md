# Задание 2

Создание образа:
docker build -t stocksproducts:1 .

Запуск контейнера:
docker container run -d -p 8000:8000 stocksproducts:1
