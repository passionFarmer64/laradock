ARG WEBGRIND_VERSION=latest
FROM clue/webgrind:${WEBGRIND_VERSION}

#####################################
# Set Timezone
#####################################

USER root

# ARG TZ=UTC
# ENV TZ ${TZ}

EXPOSE 15777

#####################################
# install from github (newest)
#####################################
# RUN mkdir -p /var/www
WORKDIR /var/www
COPY ./webgrind/ /var/www/
