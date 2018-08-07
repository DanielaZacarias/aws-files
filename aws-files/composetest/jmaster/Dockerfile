FROM jenkins/jenkins:lts

# Copy the file that will install the plugins
COPY install-plugins.sh /usr/local/bin/install-plugins.sh
RUN whoami; ls -la /usr/local/bin/; chmod 755 "/usr/local/bin/install-plugins.sh"

# Add/Remove the plugins you want
RUN /usr/local/bin/install-plugins.sh swarm
