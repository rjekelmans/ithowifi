FROM python:3.8-slim-buster

# Upgrade pip
RUN python -m pip install --upgrade pip

# Install python packages
COPY requirements.txt /tmp/pip-tmp/
RUN pip3 --disable-pip-version-check --no-cache-dir install -r /tmp/pip-tmp/requirements.txt \
    && rm -rf /tmp/pip-tmp
