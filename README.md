##  Counter-strike: Source Dedicated Server Images
*NOT AN OFFICIAL IMAGE.*<br/>

### Pull from DockerHub
```bash
docker pull fnjn/css:latest
docker run -d -p 27015:27015 css:latest
```

### Build from Dockerfile
```bash
git git@github.com:Fnjn/css-docker.git
cd css-docker
docker build . -t css:latest
docker run -d -p 27015:27015 css:latest
```

### Configuration
Configure server setting in `cfg/server.cfg`.<br/>
Add banned IP in `cfg/listip.cfg`.<br/>
Add banned users in `cfg/banned.cfg`.<br/>

### Example
Run bomb-defuse mode on de_dust2 with maximum 32 players.
```
./hlds_run -game cstrike +maxplayers 32 +map de_dust2 +hostname "Counter-Strike Dedicated Server"
```
*note: first exec after setup usually fails, simply run the command again.*

<br/>**Report any problem to issue page.**<br/>
