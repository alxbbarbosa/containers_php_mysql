# Container para desenvolvimento de projeto

Caso apresentar aviso de memória:
```
WARNING: Some services (web) use the ‘deploy’ key, which will be ignored. Compose does not support ‘deploy’ configuration — use `docker stack deploy` to deploy to a swarm.
```
Essa mensagem é exibida porquê o docker-compose na versão 3.x não suporta a chave de deploy. Então, deve-se executar o docker no modo swarm ou utilizar o comando:

```
docker-compose --compatibility up -d
```
