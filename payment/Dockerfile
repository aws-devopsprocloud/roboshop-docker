# FROM python:3.9 
# EXPOSE 8080
# WORKDIR /opt/server
# COPY payment.ini /opt/server
# COPY *.py /opt/server
# COPY requirements.txt /opt/server
# RUN pip3 install -r requirements.txt
# CMD ["uwsgi", "--ini", "payment.ini"]

FROM python:3.9.23-alpine3.22
EXPOSE 8080
ENV AMQP_USER=roboshop \
    AMQP_PASS=roboshop123

WORKDIR /app 
COPY requirements.txt /app 
RUN pip3 install -r requirements.txt
COPY *.py /app/
COPY payment.ini /app/ 
CMD ["uwsgi", "--ini", "payment.ini"]
