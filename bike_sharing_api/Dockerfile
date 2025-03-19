FROM python:3.10-slim

WORKDIR /app

RUN apt-get update && apt-get install -y wget

COPY requirements.txt ./

RUN pip install --no-cache-dir -r requirements.txt

RUN wget "https://github.com/Bluthunder/bikesharemodel/releases/download/v0.1.0/bikeshare_rental_model-0.1.0-py3-none-any.whl" && \
    pip install bikeshare_rental_model-0.1.0-py3-none-any.whl

COPY . .

EXPOSE 7070

CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "7070"]
