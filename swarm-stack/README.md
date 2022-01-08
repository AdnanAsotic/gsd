# Swarm stack

Python flask app:
- stores counter in redis
- returns count and hostname of contriner servicing request

Deploy

sudo docker stack deploy -c docker-compose.yml counter

List

sudo docker stack ps counter


