FROM node:14.18.1-buster

RUN \
  echo "**** Pulling from git ****" && \
  cd / && \
  git clone https://github.com/RallerenP/statify.git && \
  echo "**** Creating Start Script ****" && \
  echo "cd /statify/backend && git checkout \${GIT_BRANCH} && git pull && yarn install && yarn build && yarn start" >> start && \
  chmod +x start
