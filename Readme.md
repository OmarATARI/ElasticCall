# Get started

## Prerequites

- Docker installed
- docker-compose

## Expand the maximum memory

- Windows:
```
docker-machine ssh
sudo sysctl -w vm.max_map_count=262144
exit
```

- Unix
```
sudo sysctl -w vm.max_map_count=262144
```

## Check cluster state
- curl http://localhost:9200/_cat
- curl http://localhost:9200/_cat/indices
- curl http://localhost:9200/_cluster/health/?pretty 
