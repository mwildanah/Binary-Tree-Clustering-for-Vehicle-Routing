# python base 3.7 slim-buster
FROM python:3.7-slim-buster

# update ubuntu
RUN apt-get -y update

# copy requirements file
COPY . /usr/workspace

# install requirements lib
RUN apt-get install -y libssl-dev libpq-dev python-dev gcc
RUN pip install google-oauth
RUN pip install --upgrade google-api-python-client

WORKDIR /usr/workspace
RUN pip install -r requirements.txt
