FROM circleci/golang:1.15.2
ENV PS1='🐳 > '

USER root

RUN curl https://releases.hashicorp.com/terraform/0.13.4/terraform_0.13.4_linux_amd64.zip -o terraform_0.13.4_linux_amd64.zip \
  && unzip terraform_0.13.4_linux_amd64.zip \
  && mv terraform /usr/bin \
  && rm terraform_0.13.4_linux_amd64.zip

USER circleci
