FROM jenkins/jenkins:lts

# Switch to root to install additional packages or plugins
USER root

# Example: install git and curl
RUN apt-get update && apt-get install -y git curl && rm -rf /var/lib/apt/lists/*

# Switch back to Jenkins user
USER jenkins

# Example: install Jenkins plugins (optional)
# You can add a plugins.txt file listing plugins and use the install-plugins.sh script
# COPY plugins.txt /usr/share/jenkins/plugins.txt
# RUN jenkins-plugin-cli --plugin-file /usr/share/jenkins/plugins.txt