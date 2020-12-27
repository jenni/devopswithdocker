FROM ubuntu:16.04

WORKDIR /mydir
RUN apt-get update && apt-get install -y curl

COPY script.sh .
RUN chmod 755 script.sh

CMD ["./script.sh"]
