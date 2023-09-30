For future personal consults:

- Volumes only exists in "docker-compose.yaml" , they will make possible development mode


## After creating a Dockerfile you need to transform it into a image:
docker build -t myuser/express:1.1  .

docker run -p 3000:3000 -d myuser/express:1.1

##### .dockerignore
Only for developing projects when you have local node_modules, when you copy COPY . . node modules also is copied, but it's runned npm install, don't need to copy it.

##### docker.hub
 Login: docker login (user + pass)
 docker build -t user/imageName:1.1  .
 docker push user/imageName:1.1
