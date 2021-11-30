FROM cimg/go:1.16

# Docker now uses buildkit, and so the output of commands is not visible.
# To make the output visible, which only works for non-cached commands, 
#   docker build --progress=plain .

RUN whoami

ENV PS1='🐳 > '
ENV NODE_VERSION=16.13.0-deb-1nodesource1
ENV TERRAFORM_VERSION=0.13.4


USER root

RUN curl https://releases.hashicorp.com/terraform/${TERRAFORM_VERSION}/terraform_${TERRAFORM_VERSION}_linux_amd64.zip -o terraform_${TERRAFORM_VERSION}_linux_amd64.zip \
  && unzip terraform_${TERRAFORM_VERSION}_linux_amd64.zip
RUN sudo mv terraform /usr/bin
RUN rm terraform_${TERRAFORM_VERSION}_linux_amd64.zip
RUN [ "/bin/bash", "-c", "echo", "Terraform Version: $(terraform --version)" ]

# RUN mkdir -p /root/.ssh/
# RUN echo -e "Host github.com\n\tStrictHostKeyChecking no\n" >> /root/.ssh/config

# adding the go executable directory to the root user path
# https://unix.stackexchange.com/questions/228314/sudo-command-doesnt-source-root-bashrc
#RUN echo "PATH=${PATH}" > /root/.profile
#USER circleci

# https://github.com/nodesource/distributions
RUN curl -fsSL https://deb.nodesource.com/setup_16.x | sudo -E bash -
RUN sudo apt-get install -y nodejs=${NODE_VERSION}
#RUN apt-get install -y nodejs
RUN echo "Node Version: $(node -v)"

RUN curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64-2.1.36.zip" -o "/tmp/awscliv2.zip"
RUN unzip /tmp/awscliv2.zip -d /tmp/
RUN /tmp/aws/install

RUN echo aws --version

# Postgres client
RUN apt-get install postgresql-client
RUN echo psql --version

# Flyway
RUN wget -qO- https://repo1.maven.org/maven2/org/flywaydb/flyway-commandline/8.1.0/flyway-commandline-8.1.0-linux-x64.tar.gz | tar xvz && sudo ln -s `pwd`/flyway-8.1.0/flyway /usr/local/bin 
RUN flyway --version

# USER circleci