# mega-minecraft
megabrain minecraft server

# if you are Player
read this.
## install modes
```shell
# mac version
cd ~/.minecraft/mods
while IFS = read -r line
do
  line=$(echo $line | sed -e 's/#.*//') # remove comments
  if [ ! "$line" ]; then continue; fi # skip empty lines
  curl -O "$line" # download mod from cdn
done < "mods.txt"
```

# if you are Server Owner
read this.
- [itzg/docker-minecraft-server](https://github.com/itzg/docker-minecraft-server)

## run minecraft server detached mode
```shell 
docker compose up -d
```

## check minecraft server status
```shell
docker compose ps
```

## check minecraft server logs
```shell
docker compose logs -f
```

## stop minecraft server
```shell
docker compose down
```
