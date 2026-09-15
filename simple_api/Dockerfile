FROM python:3.11-bookworm
LABEL maintainer="Hassan ANEZMI"
COPY requirements.txt student_age.py /
RUN apt update -y && apt install -y python3-dev libsasl2-dev libldap2-dev libssl-dev
RUN pip3 install -r /requirements.txt
VOLUME [ "/data" ]
EXPOSE 5000
CMD [ "python3", "./student_age.py" ]