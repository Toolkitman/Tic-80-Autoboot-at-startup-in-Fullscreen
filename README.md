# Tic-80-Autoboot-at-startup-in-Fullscreen
How to make Tic-80 Autoboot at startup in Fullscreen
Hello Here is Toolkitman!
My idea was to make a real computer inspired over the TIC-80 Phantasy Computer software,
so i have think why not use the raspberry pi distribution and make it bootable at startup 
in fullscreen, the result is a working TIC-80 computer.

Here the move to do it:

go to this link https://tic80.com/create

and download this distribution in your raspbian distro : Raspberry PI	tic80-v0.90-rpi.deb	2.81MB

click over it and follow instructions to install it.

while installed reboot write in terminal tic80 to try if it works.

Now make it start at boot:


write this in terminal: sudo nano /home/pi/.config/autostart/clock.desktop

and copy paste this code with mouse click 

[Desktop Entry]
Type=Application
Name=TIC-80
Exec=/usr/bin/tic80 --fullscreen

press control X and Yes and return

go to the raspberry menu and open preferences-Main menu editor-Preferences and mark the Desktop Session Settings

click ok

Go to Menu Preferences-Desktop Session Settings-and mark TIC-80


reboot

It should go!!!!

Enjoy your new TIC-80 Computer

To close it press F11 and leave the tic80 windows open, then click shutdown.

The MIT License (MIT)
Copyright © 2022 <copyright holders>

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.


