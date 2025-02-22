<!--
N.B.: This README was automatically generated by https://github.com/YunoHost/apps/tree/master/tools/README-generator
It shall NOT be edited by hand.
-->

# Minecraft for YunoHost

[![Integration level](https://dash.yunohost.org/integration/minecraft.svg)](https://dash.yunohost.org/appci/app/minecraft) ![Working status](https://ci-apps.yunohost.org/ci/badges/minecraft.status.svg) ![Maintenance status](https://ci-apps.yunohost.org/ci/badges/minecraft.maintain.svg)  
[![Install Minecraft with YunoHost](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=minecraft)

*[Lire ce readme en français.](./README_fr.md)*

> *This package allows you to install Minecraft quickly and simply on a YunoHost server.
If you don't have YunoHost, please consult [the guide](https://yunohost.org/#/install) to learn how to install it.*

## Overview

Minecraft is a sandbox construction game, whose gameplay involves players interacting with the game world by placing and breaking various types of blocks in a three-dimensional environment. In this environment, players can build creative structures, creations, and artwork on multiplayer servers and singleplayer worlds across multiple game modes.

### Supported Servers
 
1. Minecraft (Vanilla)
2. Minecraft (Vanilla snapshot)
3. Spigot
4. Paper


**Shipped version:** 1.19.2~ynh2

## Disclaimers / important information

## Configuration

For server administration, use the Minecraft console or mcrcon (which is open on port 25575 and uses the password chosen during the install).

To use mcrcon, go to `/var/www/minecraft/mcrcon` and type:
```
./mcrcon -p YourPassword command
```
where `command` is a standard Minecraft command. You must use quotes if your command contains spaces.

You can find more info about the usage of mcrcon here: https://github.com/Tiiffi/mcrcon

The **gamemode** and the **world seed** can be set in the config panel, in the webadmin.
Other settings can be set by modifying `/var/www/minecraft/server.properties`.
## Documentation and resources

* Official app website: <https://www.minecraft.net/>
* Official admin documentation: <https://minecraft.fandom.com/wiki/Tutorials/Setting_up_a_server>
* YunoHost documentation for this app: <https://yunohost.org/app_minecraft>
* Report a bug: <https://github.com/YunoHost-Apps/minecraft_ynh/issues>

## Developer info

Please send your pull request to the [testing branch](https://github.com/YunoHost-Apps/minecraft_ynh/tree/testing).

To try the testing branch, please proceed like that.

``` bash
sudo yunohost app install https://github.com/YunoHost-Apps/minecraft_ynh/tree/testing --debug
or
sudo yunohost app upgrade minecraft -u https://github.com/YunoHost-Apps/minecraft_ynh/tree/testing --debug
```

**More info regarding app packaging:** <https://yunohost.org/packaging_apps>
