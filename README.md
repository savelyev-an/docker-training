# docker-training
Материальчики для тренинга по докеру

#sample1
находясь в каталоге sample1 
1) запускаем приложение: python app.py 
   заходим браузером http:\\localhost:5000\ - убеждаемся что приложение работает 
   останавливаем приложение
2) строим образ докер: docker build -t my_docker_flask:latest .
   запускаем контейнер: docker run -d  my_docker_flask:latest
   Задача - добиться того, чтобы по адресу http:\\XXX.XXX.XXX.XXX:5000\ был доступен hello world
3) После выполнения задачи 1 - останавливаем контейнер командой docker stop
   Запускаем приложение python app.py
   Пробуем запустить контейнер: docker start - убеждаемся что из-за занятого 5000 порта контйенер не стартует. Бывает срывается автодеплой и запуск докер-compose из-за того что порт занят старым контейнером
   
   
