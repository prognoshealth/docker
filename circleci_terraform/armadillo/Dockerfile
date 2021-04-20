FROM circleci/golang:1.15.2
ENV PS1='🐳 > '

USER root

RUN curl https://releases.hashicorp.com/terraform/0.13.4/terraform_0.13.4_linux_amd64.zip -o terraform_0.13.4_linux_amd64.zip \
  && unzip terraform_0.13.4_linux_amd64.zip \
  && mv terraform /usr/bin \
  && rm terraform_0.13.4_linux_amd64.zip

RUN curl -sL https://deb.nodesource.com/setup_15.x | sudo -E bash -
RUN sudo apt-get install -y nodejs=15.14.0-1nodesource1

RUN curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64-2.1.36.zip" -o "awscliv2.zip"
RUN unzip awscliv2.zip
RUN sudo ./aws/install

USER circleci
