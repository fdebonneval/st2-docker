FROM ubuntu:14.04

RUN apt-get update && \
    apt-get install -y curl apt-transport-https
RUN curl https://bintray.com/user/downloadSubjectPublicKey?username=bintray | sudo apt-key add -
RUN echo "deb https://dl.bintray.com/stackstorm/trusty_staging unstable main" | sudo tee /etc/apt/sources.list.d/st2-stable.list
RUN apt-get update && \
    apt-get install -y st2

EXPOSE 9091
