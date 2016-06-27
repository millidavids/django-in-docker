FROM python:3.5
MAINTAINER david.a.yurek@gmail.com

RUN apt-get update && \
	apt-get install -y python3-pip python3-dev libpq-dev
RUN pip3 install Django

ENV appdir /home/app
ADD . ${appdir}
WORKDIR ${appdir}

CMD ["python3", "manage.py", "runserver", "0.0.0.0:80"]
