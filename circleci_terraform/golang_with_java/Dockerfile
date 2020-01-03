FROM circleci/golang:1.12.9

USER root

RUN curl https://releases.hashicorp.com/terraform/0.12.7/terraform_0.12.7_linux_amd64.zip -o terraform_0.12.7_linux_amd64.zip \
  && unzip terraform_0.12.7_linux_amd64.zip \
  && mv terraform /usr/bin \
  && rm terraform_0.12.7_linux_amd64.zip

RUN apt-get update
RUN apt-get install default-jre

USER circleci