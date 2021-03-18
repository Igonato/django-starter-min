FROM python:latest
ENV PYTHONUNBUFFERED=1
ENV PIPENV_KEEP_OUTDATED=1
WORKDIR /app
COPY Pipfile Pipfile.lock /app/
RUN pip install pipenv
RUN pipenv install --dev --system
COPY . /app/
