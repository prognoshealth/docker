
FROM circleci/ruby:2.4.3
USER circleci
ARG TERRAFORM_VERSION
ARG KITCHEN_TERRAFORM_VERSION

ENV TERRAFORM_VERSION ${TERRAFORM_VERSION:-0.11.7}
ENV KITCHEN_TERRAFORM_VERSION ${KITCHEN_TERRAFORM_VERSION:-3.3.0}

RUN gem install kitchen-vagrant
RUN gem install kitchen-ansible
RUN gem install kitchen-inspec
RUN gem install awspec
RUN gem install kitchen-terraform --version ${KITCHEN_TERRAFORM_VERSION}
RUN gem install kitchen-verifier-awspec
RUN gem install rspec_junit_formatter
RUN sudo wget https://releases.hashicorp.com/terraform/${TERRAFORM_VERSION}/terraform_${TERRAFORM_VERSION}_linux_amd64.zip
RUN sudo unzip terraform_${TERRAFORM_VERSION}_linux_amd64.zip
RUN sudo mv terraform /usr/bin

ENV AWS_ACCESS_KEY_ID=""
ENV AWS_SECRET_ACCESS_KEY=""
ENV AWS_DEFAULT_REGION="us-east-1"

EXPOSE 80

CMD ["/bin/sh"]