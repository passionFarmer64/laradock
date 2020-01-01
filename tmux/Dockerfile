ARG TMUX_VERSION=latest
FROM taisun/tmux:${TMUX_VERSION}

#####################################
# Set Timezone
#####################################

ARG TZ=UTC
ENV TZ ${TZ}

COPY ./.tmux.conf ~/.tmux.conf

USER root

RUN apt-get update && apt-get install -y git
RUN mkdir -p ~/.tmux/plugins/tpm
WORKDIR ~/.tmux/plugins/tpm
RUN cd ~/.tmux/plugins/tpm \
    && git clone https://github.com/tmux-plugins/tpm.git \
    && tmux source ~/.tmux.conf \