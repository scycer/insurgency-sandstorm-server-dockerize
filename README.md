## Server Docs

https://docs.google.com/document/d/1GDLg5p9jjeIya7EgBk0ibzDtDlyQ-U_jpspOzby-JmM/edit

## How to build

```
docker build --no-cache -t scycer/insurgency-sandstorm .
```

## How to launch

```
docker run -it --rm --net=host -e HOSTNAME="Sketchland" -e PASSWORD="balls" -e GROUP="Mountain" -e MAP="Scenario_Summit_Checkpoint_Security" --name=sandstorm-dedicated --volume /home/scycer/development/insurgency-sandstorm-server-dockerize/config/ini/Engine.ini:/home/steam/steamcmd/sandstorm/Insurgency/Saved/Config/LinuxServer/Engine.ini:ro --volume /home/scycer/development/insurgency-sandstorm-server-dockerize/config/ini/Game.ini:/home/steam/steamcmd/sandstorm/Insurgency/Saved/Config/LinuxServer/Game.ini:ro --volume /home/scycer/development/insurgency-sandstorm-server-dockerize/config/txt/MapCycle.txt:/home/steam/steamcmd/sandstorm/Insurgency/Config/Server/MapCycle.txt:ro scycer/insurgency-sandstorm
```

# RCON CLI

```
rcon -H 0.0.0.0 -p 29099 -P balls
```

travel PowerPlant
travelscenario Scenario_PowerPlant_Checkpoint_Security
travelscenario Scenario_Ministry_Checkpoint_Security
gamemodeproperty MinimumEnemies 15
gamemodeproperty MaximumEnemies 15

gamemodeproperty MinimumEnemies 30
gamemodeproperty MaximumEnemies 30
