FROM python:3.10-slim

WORKDIR /app
RUN pip install pipenv

COPY Pipfile Pipfile.lock ./

RUN pipenv install --system


COPY . .

EXPOSE 5000
CMD ["python", "app.py"]
