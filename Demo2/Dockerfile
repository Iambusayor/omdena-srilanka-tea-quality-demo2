FROM python:3.8-slim 

WORKDIR /app

COPY requirements.txt ./requirements.txt

RUN pip install --no-cache-dir -r requirements.txt

EXPOSE 8501
EXPOSE 80

COPY . /app

ENTRYPOINT [ "streamlit", "run" ]

CMD [ "app.py" ]