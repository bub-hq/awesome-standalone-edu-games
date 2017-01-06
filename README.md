# Awesome Standalone Educational Games

List of awesome educational games and resources that can be turned into stand alone applications.

## Ready to package
These applications or games are already standalone and run off a native system - they just need a healthy dose of Docker package to make them easy to deploy.
* Quite a long list of applications that can be easily shipped on top of a Kivy base and are touch-ready (mostly written for Android / iOS, but run on any Python platform) : https://github.com/kivy/kivy/wiki/List-of-Kivy-Projects

## Needs rework
These applications would need a code rework or adaptation to make them work as standalone apps (for instance, a node.js starter wrapper etc...)

## Would be nice to have
These applications are not suitable as such, but would be nice to have or support in some way (may need to write a client program, change or adapt the resolution, make them touch-friendly).

* Physics-based games 
    * PHET : Physics simulations - e.g. State of matter - Problem : the resolution is fixed and not touch-friendly. Example : 
https://phet.colorado.edu/sims/html/states-of-matter-basics/latest/states-of-matter-basics_en.html
* A websockets enabled fridge magnet application - All member of a given community can drag letters or words to compose sentences. Still looking for a free one, it would require peer-to-peer or a central websocket server.
* Hardware accelerated full-screen media player such as  Gnome-mplayer comes recommended on the CHIP (Mpv would be nice https://mpv.io/ ); Alternatives are :
    * Another option would be https://vlc-qt.tano.si/ to create a simple full-screen media player
    * HPlayer https://github.com/Hemisphere-Project/HPlayer
    * Or go for an already Dockerized application (to be adapted for armhf though) https://github.com/wernight/docker-mopidy
* Background music player (to play while other apps are running, to trigger alarm actions).

# Random Musings 

## Google Material Design support across the board
It would be nice to keep a consistent look and feel across apps and UIs. Google Material Design (MD) principles are gaining traction and offer a clean and visually pleasing experience. Some existing MD skins for various UI platforms :

* Kivy : https://gitlab.com/kivymd/KivyMD
* JavaFX : http://www.jfoenix.com/ 
* Qt QML : https://github.com/papyros/qml-material

## Similar solutions

* Android App Inventor (and a plethora of similar solutions) - Generate applications for the Android platform.
* Microsoft TouchDevelop (https://www.touchdevelop.com/platforms) - Targets HTML 5 platforms only (coding using blocks that translate to Javascript) - TouchDevelop can target the BBC Microbit and can be used to make interactive tutorials.
* GoMix (http://gomix.com) - Limited to online apps and node.js at the moment.

## Adaptation ideas :
* Run Chromium and Pepper Flash - applications can be simple URLs to existing web resources (implies connectivity) or locally running ones : https://bbs.nextthing.co/t/chromium-on-chip-pepper-flash/2364/3 

## Supported pre-packaged dependency starting points

The following Github repo provides barebones programming language containers (x86 container unfortunately, but easy to adapt) : https://github.com/nacyot/docker-programming-languages

* PyQt5 + QML + Multimedia support
* QtWebView + Web application (served locally ?)
* RenPy : Should support Blockly to make Renpy scripts and allow to run them simply.
    * No support for armhf yet, but instructions exist : https://dlksk.tumblr.com/post/107500026059/getting-renpy-to-run-on-the-raspberry-pi
* PygameZero + Pymunk for physics-based games
* Kivy
* Processing.org
* node.js
* JavaFX
    * Diozero : Interesting Java 8 with a CHIP port on the way (https://github.com/mattjlewis/diozero)
    * JavaFX Material Design UI lib : http://www.jfoenix.com/ 
* Lua / (Pico8 ?)
* Chromium + Flash
