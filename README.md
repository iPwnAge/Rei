# Rei

<img src="http://i.imgur.com/4JoNdAe.png" height="100px">


![Minecraft Forge v10.13.4.1614][forge]
![Minecraft v1.7.10][mc]
![Java JDK v1.8][java]
![Spigot 1.7.10 Snapshot ][spigot]

### What's Rei?
Rei is a fork of Thermos, a craftbukkit forge server for Minecraft 1.7.10. It seeks to improve performance on the already lean Thermos, as well as fine tuning specific to the iPwnAge Network FTB server. 

Advantages over KCauldron:
+ Lag-lowering optimizations
+ Better world protection (Forge stuff doesn't bypass Bukkit plugins!)
+ Many patches that KCauldron didn't get from Spigot
+ Dupe glitch fixes

**Because of it's specific usage for the iPA Network, you should not expect Rei to work in your environment.**


## Build Requirements
* Java 8u101 JDK or higher
* `JAVA_HOME` defined on your OS

## Building Rei
* Checkout project
  * You can use IDE or clone from console:
  `git clone https://github.com/iPwnAge/Rei.git`
* Setup
  * Auto: `setup.sh`
  * Manual:
  `git submodule update --init --recursive`
* Build
  * This process downloads minecraft and apply patches
  * If you have gradle integration in IDE - you can still use gui
  * Auto: `build.sh`
  * Manual:
  `./gradlew setupCauldron jar`

All builds will be in `build/distributions`
  
## Updating sources
* Update sources
  * `git pull origin master`
* Re apply patches & build binaries
  * `./gradlew clean setupCauldron jar`
