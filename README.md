![](https://github.com/AndrewMarchukov/insurgency-sandstorm-server-dockerize/blob/master/sandstorm-logo.png)
![](https://github.com/AndrewMarchukov/insurgency-sandstorm-server-dockerize/blob/master/docker-logo.jpg)
## How to build
```
docker build -t scycer/insurgency-sandstorm .
```

## How to launch
```
docker run -it --rm --net=host -e HOSTNAME="Sketchland" -e PASSWORD=balls --name=sandstorm-dedicated --volume /home/scycer/development/insurgency-sandstorm-server-dockerize/config/ini/Engine.ini:/home/steam/steamcmd/sandstorm/Insurgency/Saved/Config/LinuxServer/Engine.ini:ro --volume /home/scycer/development/insurgency-sandstorm-server-dockerize/config/ini/Game.ini:/home/steam/steamcmd/sandstorm/Insurgency/Saved/Config/LinuxServer/Game.ini:ro --volume /home/scycer/development/insurgency-sandstorm-server-dockerize/config/txt/MapCycle.txt:/home/steam/steamcmd/sandstorm/Insurgency/Config/Server/MapCycle.txt:ro scycer/insurgency-sandstorm
```

