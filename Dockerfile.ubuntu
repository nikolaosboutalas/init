FROM ubuntu:latest

RUN apt-get update && \
    apt-get install -y ansible python3-apt

RUN apt-get install -y sudo \
    && useradd -m -s /bin/bash admin \
    && echo "admin ALL=(ALL) ALL" >> /etc/sudoers \
    && passwd -d root

RUN echo 'admin:admin' | chpasswd

USER admin
WORKDIR /home/admin

COPY --chown=admin . init
WORKDIR init

CMD ["/bin/bash"]
