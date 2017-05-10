FROM python:3.3-slim
MAINTAINER Torben Brodt <t.brodt@gmail.com>

RUN mkdir -p /usr/src/app
COPY extruct /usr/src/app/extruct
WORKDIR /usr/src/app/extruct

RUN pip3 install extruct
RUN pip3 install -r requirements.txt

ENTRYPOINT ["python3"]
CMD ["-m", "extruct.service"]
