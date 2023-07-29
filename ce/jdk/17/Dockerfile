FROM ghcr.io/graalvm/jdk:ol9-java17-22.3.3

LABEL author="Sersoid"

RUN useradd -d /home/container -m container

USER container
ENV USER=container HOME=/home/container
WORKDIR /home/container

COPY ../../../entrypoint.sh /entrypoint.sh
CMD [ "/bin/bash", "/entrypoint.sh" ]
