FROM ubuntu

RUN apt-get update && \
    apt-get upgrade -y && \
    apt-get install git -y

ADD entrypoint.sh /entrypoint.sh

RUN chmod +x entrypoint.sh

ENTRYPOINT [ "/entrypoint.sh" ]