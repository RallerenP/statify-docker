FROM node:14.18.1-buster

RUN \
  echo "**** Pulling from git ****" && \
  cd / && \
  git clone https://github.com/RallerenP/statify.git && \
  echo "**** Installing Dependencies ****" && \
  cd statify/frontend && \
  yarn install && \
  echo "**** Building Statify Frontend ****" && \
  yarn build && \
  echo "**** Creating Start Script ****" && \
  cd / && \ 
  echo "cd /statify/frontend && yarn start" >> start && \
  chmod +x start
