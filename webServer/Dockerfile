FROM node:alpine

WORKDIR /usr/app

# Copy only package.json for caching
COPY ./package.json ./
RUN npm install

# Copy from root to /usr/app in container
COPY ./ ./

CMD ["npm","start"]

# Docker build -t dockerID/imageName .
# Docker run -p 8080:8080 dockerID/imageName
# Docker run -it dockerID/imageName sh
