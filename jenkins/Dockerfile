FROM jenkins/jenkins:lts

USER root

RUN apt-get update && apt-get install -y curl && \
    curl -L https://download.docker.com/linux/static/stable/x86_64/docker-20.10.24.tgz -o docker.tgz && \
    tar -xzf docker.tgz --strip 1 -C /usr/local/bin docker/docker && \
    rm docker.tgz

USER jenkins