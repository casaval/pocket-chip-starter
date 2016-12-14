# pocket-chip-starter
A single download of configs to get a Pocket C.H.I.P. up and running

Note: Commands will be listed in the readme but will (eventually) be available as separate scripts so this repo can be checked out on the PocketCHIP directly and have those available.

# Update pocket chip (do before any of these game installs)
```
sudo apt update && sudo apt install
sudo apt install git
```

# Doom
Install
```
sudo apt install prboom doom-wad-shareware
```
Run Multiplayer
```
prboom-game-server
prboom -net 172.20.0.1
```
Run Singleplayer
```
prboom
```

# Quake 3 Arena (Open Arena)
Install
```
git clone https://github.com/NextThingCo/ioquake3-gles
cd ioquake3-gles
./build.sh
```
Run
```
openarena
```


# Minecraft Pi Edition
Install
```
wget https://github.com/NextThingCo/chipcraft/archive/master.zip
unzip master.zip
cd chipcraft-master
./build.sh
```
Run
```
/home/chip/chipcraft-master/mcpi/start.sh
```

## Todo
# Wireless Access Point
# Configure USB Gamepad
# Quake 1
# Quake 2
# OpenRCT
# OpenTTD
