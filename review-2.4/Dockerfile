FROM cattaka/docker-review:2.4.0a
LABEL maintainer="ngtknt@me.com"

# use inconsolata
RUN apt-get update && \
    apt-get install -y --no-install-recommends \
    fonts-inconsolata xzdec wget && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*
RUN tlmgr init-usertree && \
    tlmgr update --self --all && \
    tlmgr install inconsolata
