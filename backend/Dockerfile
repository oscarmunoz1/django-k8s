FROM python:3.9.7-slim

COPY . /app
WORKDIR /app

# Create virtual environment
RUN python3 -m venv /opt/venv

# Install requirements
RUN /opt/venv/bin/pip install pip --upgrade && \
    /opt/venv/bin/pip install -r requirements.txt && \
    chmod +x entrypoint.sh

CMD ["/app/entrypoint.sh"]