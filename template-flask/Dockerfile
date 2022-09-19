FROM python:3.7

RUN apt-get update && apt-get upgrade -y && \
    pip install --upgrade pip && apt-get install -y libgl1-mesa-dev

WORKDIR /backend

COPY ./backend /backend

RUN pip3 install -r requirements.txt