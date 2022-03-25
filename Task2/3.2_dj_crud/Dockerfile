FROM python:3.8

WORKDIR /stocks_products

COPY ./stocks_products /stocks_products

RUN pip install -r requirements.txt

ENV SECRET_KEY wqevrbntjykliyuktyjrthr

ENV DEBUG True

RUN python3 manage.py migrate

EXPOSE 8000

CMD gunicorn stocks_products.wsgi -b 0.0.0.0:8000

