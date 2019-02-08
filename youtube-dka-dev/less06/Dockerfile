#  базовый образ, обязательно как самай первая инструкция
FROM ubuntu

# Не обязательная информация об авторе

MAINTAINER vitto <vitto@localhost>

# RUN = команды которые должны запускаться внутри образа

RUN apt-get update && apt-get install -y mc

# теперь надо выполнить билд ОБРАЗА
# docker build -t testimage .
# результат можно увидеть так
# docker images
# теперь можно создать и запустить контейнер
# docker run -it testimage mc

# вместо указания точки входа при создании контейнера (docker run -it testimage mc), ее можно указать тут
# аргументы по прежнему можно передавать docker run -it --name testapp testimage /etc/

ENTRYPOINT ["mc"]

