# Nodejs web app

Express app with handlebars view engine.

Login to hub:

sudo docker login

Build : 

sudo docker image build -t adnanasotic/gsd:firstcontainer .

Run:

sudo docker container run -d --name web -p 8000:8080 adnanasotic/gsd:firstcontainer

Run interactive (foreground):

sudo docker container run -it --name test alpine sh
exit to exit

View Logs:

sudo docker logs web

Stop

docker container stop web

Start

docker container start web

Delete

docker container stop web
docker container rm web

Swarm Mode

docker swarm init
call for managers and workers (3 managers - odd)

Create Service

sudo docker service create --name web -p 8000:8080 --replicas 3 adnanasotic/gsd:firstcontainer
