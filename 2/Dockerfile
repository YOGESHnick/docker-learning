FROM node
WORKDIR /app
#copy all files and subfolders in same level as Dockerfile into ./(current directory) 
COPY package.json /app
# copy package.json and then run npm install...so whenever code changes, only the code part is re-built and
# not the package.json where nothing were changed
RUN npm install
COPY . /app
EXPOSE 80
CMD ["node" , "server.js"]
# docker run -p 3000:80 [id] 