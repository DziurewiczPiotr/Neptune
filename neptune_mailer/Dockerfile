FROM docker.io/library/python:3.10

RUN pip install -U "prefect==2.14"

COPY . .

CMD [ "python", "test_flow.py" ]