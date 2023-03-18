#set base image
FROM node:14-alpine

WORKDIR /app

#install packages
COPY package.json ./
RUN npm install


#copy everything else
COPY ./ ./

#run command
CMD ["npm", "start"]