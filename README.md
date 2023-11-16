# dockercommands

# disk prunning 
docker system prune -af --volumes

# dangling images 

docker rmi $(docker images --filter "dangling=true" -q --no-trunc)
