FROM debian:stable

RUN apt-get update && apt-get install -y \
  openssh-client \
  git && \
  rm -Rf /var/lib/apt/lists/*

ADD entrypoint.sh /entrypoint.sh
RUN chmod +x /entrypoint.sh
ENTRYPOINT ["/entrypoint.sh"]
