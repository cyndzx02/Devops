FROM python:3.12

COPY . .

COPY requirements.txt .

RUN pip3 install -r requirements.txt

EXPOSE 80

CMD [ "flask", "run", "--host=0.0.0.0", "--port=80" ]