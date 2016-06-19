FROM python:3.5
MAINTAINER david.a.yurek@gmail.com

RUN pip install Django

ENV appdir /home/app
ADD . ${appdir}
WORKDIR ${appdir}

CMD ["python3", "manage.py", "runserver", "0.0.0.0:8000"]
