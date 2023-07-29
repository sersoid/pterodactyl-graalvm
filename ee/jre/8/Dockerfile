FROM container-registry.oracle.com/graalvm/enterprise:ol9-java8-21.3.7

LABEL author="Sersoid"

RUN useradd -d /home/container -m container

USER container
ENV USER=container HOME=/home/container
WORKDIR /home/container

COPY ../../../entrypoint.sh /entrypoint.sh
CMD [ "/bin/bash", "/entrypoint.sh" ]
