FROM node:14.6.0-alpine
RUN mkdir -p /var/www/nuxt
# timezone
ARG TZ
WORKDIR /var/www/nuxt
COPY ./nuxt/ /var/www/nuxt/

RUN apk update && \
  apk add git && \
  npm install -g npm && \
  npm install -g vue-cli && \
  npm install -g create-nuxt-app@2.15.0

ENV HOST 0.0.0.0

EXPOSE 3000
