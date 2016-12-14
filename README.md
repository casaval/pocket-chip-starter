# pocket-chip-starter
A single download of configs to get a Pocket C.H.I.P. up and running

Note: Commands will be listed in the readme but will (eventually) be available as separate scripts so this repo can be checked out on the PocketCHIP directly and have those available.

# DO THIS FIRST
# Update pocket chip (do before any other instructions)
```
sudo apt update && sudo apt install
sudo apt install git
```

# Pico-8
Note: Not necessary for PocketCHIPs but regular CHIPs with an HDMI dip can also install Pico-8
```
sudo apt update && sudo apt install chip-pico-8
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
More info: [http://blog.nextthing.co/heres-how-to-host-a-90s-style-doom-lan-party-using-pocketc-h-i-p/]

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
More Info: [http://blog.nextthing.co/multiplayer-fragfest-quake-iii-pocketc-h-i-p-lan-party/]

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
More Info: [http://blog.nextthing.co/play-minecraft-on-your-c-h-i-p-pocketc-h-i-p/]

# Configure USB Gamepad
Add 'chip' as a member of the input group.
```
sudo adduser chip input
```
Restart your machine.
Copy the sdl controller config file from Github.
```
cd /home/chip/.lexaloffle/pico-8
wget https://raw.githubusercontent.com/gabomdq/SDL_GameControllerDB/master/gamecontrollerdb.txt
mv gamecontrollerdb.txt /home/chip/.lexaloffle/pico-8/sdl_controllers.txt
```
When you first start pico-8, the controller will not work. You must first background the app (by pressing the home button) and then click the pico-8 icon again. It should now work.
This info works for the Buffalo Classic USB Game Pad.

## Todo
# Wireless Access Point
# Configure USB Gamepad
# Quake 1
# Quake 2
# OpenRCT
# OpenTTD
