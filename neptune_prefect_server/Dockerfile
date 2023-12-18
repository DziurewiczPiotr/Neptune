FROM docker.io/library/python:3.10

RUN pip install -U "prefect==2.14"

RUN prefect config set PREFECT_API_URL="http://127.0.0.1:4200/api"

ENTRYPOINT [ "prefect", "server", "start" ]