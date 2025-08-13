FROM ubuntu:24.10
USER root

RUN apt update
RUN apt install -y python3.13
RUN apt install -y python3-pip

COPY requirements.txt .
# RUN python3.13 -m pip install -r requirements.txt

ENV SITE_DOMAIN=hoihoi.com

WORKDIR /var

# ADD https://archive.ics.uci.edu/ml/machine-lerning-databases/iris/iris.data .
# ENTRYPOINT xxxx

COPY script.py .
ENTRYPOINT ["python3.13", "script.py"]