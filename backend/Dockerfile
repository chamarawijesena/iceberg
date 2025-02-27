
#
#ENTRYPOINT ["top", "-b"]


# Use official Python image
FROM python:3.12
LABEL authors="chama"

WORKDIR /app
COPY requirements.txt .
RUN pip install -r requirements.txt
COPY . .
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]
