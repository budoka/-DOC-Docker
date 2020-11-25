# -DOC-Docker

#### `Dockerfile`: Script of instructions that is used to create a container image.
#### Example:

```dockerfile
FROM node:12-alpine
WORKDIR /app
COPY . .
RUN yarn install --production
CMD ["node", "src/index.js"]
```

  
##### `docker build/update (-d) (-p <port>:<port>) (-t <image tag>) .`   
`build new image (-d: run the container in detached mode -background-). (-p <port>:<port>: map port 80 of the host to port 80 in the container). (-dp 80:80). (-t <image-name>: tag the image). (.: The . at the end of the docker build command tells that Docker should look for the Dockerfile in the current directory)`

##### `docker run -dp 3000:3000 my-image`
`run new container`

##### `docker ps`
`list of containers`

##### `docker stop <the-container-id>`
`stop container`
  
##### `docker rm (-f) <the-container-id>`
`remove container. (-f: stop and remove container)`

##### `docker rm (-f) <the-container-id>`
`remove container. (-f: stop and remove container)`
