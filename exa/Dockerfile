FROM abh1nav/rust:1.23.0

# Clone the git repo, checkout v0.8.0 (commit 877265b) and build the binary
RUN cd /root && \
    git clone https://github.com/ogham/exa && \
    cd /root/exa && \
    git checkout 877265b && \
    cargo build --release --no-default-features

WORKDIR /root/exa
VOLUME /output

CMD ["cp", "/root/exa/target/release/exa", "/output/"]
