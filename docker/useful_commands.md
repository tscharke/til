# Useful commands
## List container
```shell
docker ps
```

## Stop all containers
```shell
# Smoothly
docker kill $(docker ps -a -q) 

# Brute force
docker kill $(docker ps -q)
```

[Source](https://gist.github.com/evanscottgray/8571828)
