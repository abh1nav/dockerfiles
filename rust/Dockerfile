FROM ubuntu:artful

# Install deps
RUN apt-get update && apt-get install curl git make build-essential -y

# Copy the installer
ADD ./install.sh /tmp/

# Install rust
RUN /tmp/install.sh -y

# Env var setup
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/root/.cargo/bin

CMD ["/bin/bash"]
