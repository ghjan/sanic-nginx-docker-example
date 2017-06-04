# FROM python:3.6-onbuild
#
# NOTE: THIS DOCKERFILE IS GENERATED VIA "update.sh"
#
# PLEASE DO NOT EDIT IT DIRECTLY.
#

FROM python:3.6

RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

ONBUILD RUN mkdir -p  ~/.pip
ONBUILD COPY pip.conf ~/.pip/
ONBUILD COPY requirements.txt /usr/src/app/
ONBUILD RUN pip install --no-cache-dir -r requirements.txt

ONBUILD COPY . /usr/src/app
