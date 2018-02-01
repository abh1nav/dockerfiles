FROM ubuntu:artful

# Install deps
RUN apt-get update && apt-get install curl -y

# Copy the installer
ADD ./install.sh /tmp/

# Install rust
RUN /tmp/install.sh -y

CMD ["/bin/bash"]
