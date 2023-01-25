FROM ubuntu

RUN apt udate \
    apt install -y git

ADD entrypoint.sh /entrypoint.sh

RUN chmod +x entrypoint.sh

ENTRYPOINT [ "/entrypoint.sh" ]