# SnakePaper
<br>
<img src="https://github.com/Xses-1/SnakePaper/blob/main/Peek%202021-12-05%2018-13.gif"> </img>
<br>
<br>
The main part is <a href="https://github.com/Code-Bullet"> Code Bullet's </a> snake from his website, which is actually P5 library for javascript + <a href="https://johnflux.com/2015/05/02/nokia-6110-part-3-algorithms/"> John Tapsells Snake solution </a>. I stripped it down, tweaked it, so it is more resource efficient, and made it work as a wallpaper using boot up scripts and stuff.<br>

<h3> What you gonna need: </h3>
* PHP dev tools<br>
  (It's needed just to start the local server because P5 will only run on a server.)<br>
  (It has a nice, easy to use, and simple dev server.)<br>
  <br>
  
  ```
  sudo apt install php
  ```
  
  <br>
* SnakePaper files from this github page<br>
<br>

```
git clone https://github.com/Xses-1/SnakePape/edit/main/README.md
```

* <a href="https://github.com/Xses-1/SnakePape/blob/main/boot_server.sh"> boot_server.sh </a> in your autostart (with the path to SnakePaper changed, so it matches the location of your SnakePaper files!)<br><br>

```
#!/bin/bash

php -S localhost:8000 -t "/home/xses/Documents/Snakepaper" & #Path to folder with your SnakePaper
```

* <a href="https://store.kde.org/p/1324580/"> HTML Wallpaper for KDE Plasma </a> or equivelent<br>
  (Direct it to http://localhost:8000)<br>
  (KDE Plasma HTML Wallpaper extension also needs Qt5 WebEngine)

```
sudo apt install qml-module-qtwebengine
```
(^---- This is recommended methode, but when I did that it actually destroyed my Plasma and now Snakepaper doesn't work anymore :( Python3 version of qt5 worked for me before)
