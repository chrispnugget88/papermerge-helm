FROM ubuntu

RUN apt-get update
RUN apt-get install -y git

ADD entrypoint.sh /entrypoint.sh

RUN chmod +x entrypoint.sh

ENTRYPOINT [ "/entrypoint.sh" ]