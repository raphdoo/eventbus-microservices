#set base image
FROM node:14-alpine

# Add the following lines
ENV CI=true
ENV WDS_SOCKET_PORT=0

WORKDIR /app

#install packages
COPY package.json ./
RUN npm install


#copy everything else
COPY ./ ./

#run command
CMD ["npm", "start"]