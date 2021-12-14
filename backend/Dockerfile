FROM node:14.18.1-buster

RUN \
  echo "**** Pulling from git ****" && \
  cd / && \
  git clone https://github.com/RallerenP/statify.git && \
  git checkout staging && \
  echo "**** Installing Dependencies ****" && \
  cd statify/backend && \
  yarn install && \
  echo "**** Building Statify Backend ****" && \
  yarn build && \
  echo "**** Creating Start Script ****" && \
  cd / && \ 
  echo "cd /statify/backend && yarn start" >> start && \
  chmod +x start
