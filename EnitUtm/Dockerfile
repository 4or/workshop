# this called the based of our image
# if you write your app in python you need to set the base into python
FROM node

# here we set the work directory inside the container
WORKDIR /usr/src/enitutm

# copy package.json and package-lock.json to /usr/src/enitutm
COPY package*.json ./

# install dependencies
RUN npm install

# copy our code 
COPY . .

# expose the port 
EXPOSE 3000
 
# run the application
CMD ["node", "user-service.js"]
