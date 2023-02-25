FROM python:3.10



WORKDIR .

COPY . .

RUN pip install poetry
RUN poetry config virtualenvs.create false && poetry install --only main



EXPOSE 5000

CMD ["python", "menu.py"]