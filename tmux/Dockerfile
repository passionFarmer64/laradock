ARG TMUX_VERSION=latest
FROM taisun/tmux:${TMUX_VERSION}

#####################################
# Set Timezone
#####################################

ARG TZ=UTC
ENV TZ ${TZ}


COPY ./.tmux.conf /root/.tmux.conf



