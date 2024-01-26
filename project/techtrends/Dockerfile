FROM python:3.8
LABEL maintainer="Marco Costa"

COPY . /app
WORKDIR /app

COPY requirements.txt .
RUN pip install -r requirements.txt
RUN python init_db.py

EXPOSE 3111

# Run on Container Start
CMD ["python", "app.py"]