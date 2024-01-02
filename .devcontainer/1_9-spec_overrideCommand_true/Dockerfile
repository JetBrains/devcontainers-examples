FROM ubuntu:latest

RUN apt-get update && apt-get install -y \
    git \
    procps \
    && rm -rf /var/lib/apt/lists/*

ENTRYPOINT ["/bin/bash", "-c", "touch /test && echo 'Hello from Dockerfile'; exec bash"]
