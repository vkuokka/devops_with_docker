FROM node:14.9.0

EXPOSE 3001
MAINTAINER vkuokka@student.hive.fi

RUN apt -y update && apt -y upgrade
RUN apt -y install git
RUN git clone https://github.com/vkuokka/helsinki-fullstack-backend.git
WORKDIR helsinki-fullstack-backend
RUN npm install
CMD ["npm", "start"]
