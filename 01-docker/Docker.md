# docker commands

nginx is smart web server.
https://hub.docker.com/_/nginx

`docker run nginx`

is it really running?

docker ps
watch docker ps

the container is completley isolated from the outside world.
including the network stack. if i want to communicate with this container
i need to map the port to the outside world.

`docker run -p 80:80 nginx`

and now we can have a look at http://localhost


we can start the docker container as deamon. that's how
how you will find container running on ceratin systems.

`docker run -p 80:80 -d nginx`


`docker ps`
`docker log [name]`
`docker log [name] --follow`

run three more nginx in background
`docker run -d nginx`
`docker run -d nginx`
`docker run -d nginx`


`docker stats`

`docker stop`

`docker cp test.txt [name]:/tmp`
`docker exec [name] ls /tmp`
`docker exec -it trusting_goldberg bash`


`docker images`
`docker ps -a`

`docker stop $(docker ps -q)`
`docker rm $(docker ps -a -q)`
