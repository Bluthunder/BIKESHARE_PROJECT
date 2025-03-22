FROM python:3.10-slim

WORKDIR /app

RUN apt-get update && apt-get install -y wget

COPY . /app

COPY requirements.txt ./

COPY ./bikeshare_model-0.0.1-py3-none-any.whl /app/

RUN pip install --no-cache-dir -r requirements.txt

RUN pip install --no-cache-dir bikeshare_model-0.0.1-py3-none-any.whl

EXPOSE 8001

CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "8001"]
