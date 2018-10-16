# VexV5Doom

This is a port of id Software's DOOM for the Vex V5 Robot Brain, using the [PROS](https://github.com/purduesigbots/pros) kernel.

It's based on floppes' [stm32doom](https://github.com/floppes/stm32doom) port and uses [Chocolate Doom](https://github.com/chocolate-doom/chocolate-doom)'s codebase.


![](https://raw.githubusercontent.com/sealj553/VexV5Doom/master/img/pic1.jpg)


![](https://raw.githubusercontent.com/sealj553/VexV5Doom/master/img/pic2.jpg)

Video: [https://www.youtube.com/watch?v=exjGBy4SHME](https://www.youtube.com/watch?v=exjGBy4SHME)


## Features
* Play with the Vex controller
* Load standard doom WAD files
* Save and load games on the microSD card (untested)

## How to use
* Clone the repo (or download .ZIP):
````
git clone https://github.com/sealj553/VexV5Doom.git
````
* Build and upload to the V5:
````
cd VexV5Doom
prosv5 make
prosv5 upload
````
* Format the microSD card to fat32 and copy "doom1.wad" to it
* Insert the microSD card and start the game

## Controls
This can be changed in `src/doom/chocdoom/i_video.c`

* left analog x = turn left/right
* left analog y = move forward/back
* right analog x = strafe left/right
* a = fire
* b = use
* x = enter
* y = escape
* dpad = arrow keys
* l1 = prev weapon
* r1 = next weapon

## Limitations
Due to hardware limitations, the following is not possible on the V5:
* Sound
* Multiplayer
* Probably other things
