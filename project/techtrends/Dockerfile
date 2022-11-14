FROM python:3.8

EXPOSE 3111

WORKDIR /app

COPY . /app

RUN pip install --upgrade pip &&\
    pip install -r requirements.txt

RUN python init_db.py

CMD ["python" , "app.py"] 