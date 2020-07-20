FROM ubuntu:16.04

RUN apt-get update -y && apt-get install -y curl
WORKDIR /mydir
COPY script.sh .
CMD ["./script.sh"]
