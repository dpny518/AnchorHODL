## Easy way to start it
Open Amazon Light Sail Server
Follow this and stop after install docker
```
https://habr.com/en/post/448108/
```
Open up ports in networking, tcp and udp

Edit Dockerfile, paste your seed phrase in the Dockerfile, where it says paste your seed phrase
update config.py for the parameters you want

Run the docker
```
docker build -t anchor .
docker run -d -p 5000:5000 anchor:latest
```
Have it restart unless stopped
get your docker id
```
docker ps
```
docker update --restart unless-stopped [docker id]
## changes made
removed 'paste seed phrase here' in config.py since it reads the seed phrase from the OS in Dockerfile

## How it works and full details
Read the original git
```
unl1k3ly/AnchorHODL
```

