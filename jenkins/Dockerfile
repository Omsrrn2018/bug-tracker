FROM jenkins/jenkins:lts

USER root

# Install dependencies for Docker install script
RUN apt-get update && apt-get install -y curl

# Install Docker CLI using official convenience script
RUN curl -fsSL https://get.docker.com -o get-docker.sh && \
    sh get-docker.sh --dry-run && \
    sh get-docker.sh && \
    rm get-docker.sh

USER jenkins