FROM python:3.10-slim

WORKDIR /project

COPY app/requirements.txt /project/requirements.txt

RUN pip install --no-cache-dir -r requirements.txt

COPY app/ /project/app/

EXPOSE 9000

CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "9000"]
