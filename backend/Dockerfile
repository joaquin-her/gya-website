ARG PYTHON_VERSION=3.12.4
FROM python:${PYTHON_VERSION}-slim as builder

# Crear directorio de trabajo
WORKDIR /app

# Copiar archivos del proyecto y dependencias con cache
RUN --mount=type=cache,target=/root/.cache/pip \
    --mount=type=bind,source=requirements.txt,target=requirements.txt \
    python -m pip install -r requirements.txt

COPY . /app

ENTRYPOINT ["python3"]
CMD ["app.py"]
