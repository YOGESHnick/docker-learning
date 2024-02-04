FROM node
WORKDIR /app
#copy all files and subfolders in same level as Dockerfile into ./(current directory) 
COPY . /app
RUN npm install
EXPOSE 80
CMD ["node" , "server.js"]