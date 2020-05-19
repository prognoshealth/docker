FROM circleci/python:3.7
ENV AWS_CLI_VERSION=1.16.260
RUN sudo pip3 install awscli==${AWS_CLI_VERSION}

FROM circleci/golang:1.12.9

USER root

RUN curl https://releases.hashicorp.com/terraform/0.12.24/terraform_0.12.24_linux_amd64.zip -o terraform_0.12.24_linux_amd64.zip \
  && unzip terraform_0.12.24_linux_amd64.zip \
  && mv terraform /usr/bin \
  && rm terraform_0.12.24_linux_amd64.zip

RUN apt-get update
RUN apt-get install default-jre

USER circleci
