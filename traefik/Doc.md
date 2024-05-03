# Traefik et autres
pswd: Bonjour@2020#
admin:$2y$05$37JIDCEi/7YjLsHvYmNbbuo9dTTpLW2n2GRHyKY31LlTdOgik.7dW

## install docker-swarm

docker swarm init --advertise-addr 10.0.0.3

 docker swarm join --token SWMTKN-1-3awlgutdo9px6udnjiur5aikw5wmg2p87muh8v89mxsalaq7je-3ujrmq3uywihlb1tb5dscy81a 10.0.0.3:2377

 Reseau pour trafik
 docker network create --driver overlay traefik-public
