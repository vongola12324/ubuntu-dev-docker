FROM ubuntu:16.04

COPY ./scripts/*.sh /tmp
RUN chmod +x /tmp/*.sh

# Install
WORKDIR /tmp
RUN bash ./install_package.sh

# Cleanup
RUN rm -Rf /tmp/*.sh
WORKDIR /

CMD ["/bin/bash"]