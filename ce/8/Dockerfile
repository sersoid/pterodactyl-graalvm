FROM ghcr.io/graalvm/graalvm-ce:ol7-java8-21

LABEL author="sersoid"

RUN useradd -d /home/container -m container

USER container
ENV USER=container HOME=/home/container
WORKDIR /home/container

COPY ../../entrypoint.sh /entrypoint.sh
CMD [ "/bin/bash", "/entrypoint.sh" ]
