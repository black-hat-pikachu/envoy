FROM python:3.10.6-slim-bullseye@sha256:b6f5aa3755f1ccdd193f5af7b04c93e8a230238580fd438040671b84fd22af7f

ADD requirements.txt /tmp/flask-requirements.txt
RUN pip3 install -qr /tmp/flask-requirements.txt
RUN mkdir /code

ENTRYPOINT ["python3", "/code/service.py"]
