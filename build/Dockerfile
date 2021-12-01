FROM node:14.18.1

EXPOSE 5432 4321 35729

ENV NPM_CONFIG_PREFIX=/usr/app/.npm-global \
    PATH=$PATH:/usr/app/.npm-global/bin

VOLUME /usr/app/spfx
WORKDIR /usr/app/spfx
RUN useradd --create-home --shell /bin/bash spfx && \
    usermod -aG sudo spfx && \
    chown -R spfx:spfx /usr/app/spfx

USER spfx

RUN npm i -g gulp-cli@2.3.0 yo@4.3.0 @microsoft/generator-sharepoint@1.13.1

CMD /bin/bash