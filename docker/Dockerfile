FROM codex-linux-dev
ARG DEBIAN_FRONTEND=noninteractive

USER root
RUN apt-get update && \
    apt-get install -y --no-install-recommends \
    npm \
    openssh-client && \
    rm -rf /var/lib/apt/lists/* && \
    npm install -g @openai/codex

USER ubuntu
