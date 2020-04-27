FROM python:3.7-alpine
WORKDIR /app
ENV FLASK_APP main.py
ENV FLASK_RUN_HOST 0.0.0.0
COPY ./src/requirements.txt /app/requirements.txt
RUN pip install -r requirements.txt
COPY ./src /app
CMD ["flask", "run"]