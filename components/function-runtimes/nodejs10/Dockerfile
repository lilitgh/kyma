# remember to deprecate this node version by april 2021 https://nodejs.org/en/about/releases/
FROM node:10.23.0-alpine3.11

LABEL source = git@github.com:kyma-project/kyma.git

COPY kubeless/ /

WORKDIR /kubeless_rt/

RUN npm install

USER 1000

CMD ["node", "kubeless.js"]