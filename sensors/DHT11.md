# DHT11

# iot Basic

### Table of Contents
=================
  * [Commands](#commands)
  * [VNC VIEWER on Mac osx:](#vnc-viewer-on-mac-osx-)
  * [AutoLogin the Raspbian](#autologin-the-raspbian)


## Commands
| command       | Description |
| ------------- |:-------------:|
| startx      	| start desktop GUI |
| hostname -I	| get ip address of pi |



## VNC VIEWER on Mac osx:

	https://smittytone.wordpress.com/2016/03/02/mac_remote_desktop_pi/
	
	sudo apt-get install tightvncserver
	
	tightvncserver
	
	# to set resolution :
	# tightvncserver -geometry 1920x1080 -depth 24

	# connect using VNC VIEWER to:
	vnc://pi.local:1

## AutoLogin the Raspbian
	https://incoherentmusings.wordpress.com/2016/04/25/setting-up-vnc-server-on-raspberry-pi-to-autostart-on-reboot/


	https://www.youtube.com/watch?v=fLtsXwdM4n0 (7:20)
	
	# type in terminal
	`sudo raspi-config`
	
	# Select in config :
	* Boot Options
	* Desktop / CLI
	* Console Autologin
	* Finish

	# go in terminal and type
	`vi ~/.bashcr`
	# add code that you wanna to run EACH time when system boot.
	# example  `tightvncserver`

## Install Camera V2 Module
	* https://www.youtube.com/watch?v=WNKbZsrsKVs 
	* https://pimylifeup.com/raspberry-pi-webcam-server/
	sudo apt-get install  libjpeg62


	* https://www.youtube.com/watch?v=ojJhLQBiv0I 
	* https://www.youtube.com/watch?v=e9PK6eLl4tM
	* `raspistill -0 image.jpg`
	* `raspivid -0  video.h264 -t 5000`

## Port forwarding:
	https://pimylifeup.com/raspberry-pi-port-forwarding/


## Problems
	* xauth timeout in locking authority file /home/pi/.xauthority  
	* http://unix.stackexchange.com/questions/215558/why-am-i-getting-this-message-from-xauth-timeout-in-locking-authority-file-ho

	* vid_v4lx_start: Failed to open video device /dev/video0     (http://raspberrypi.stackexchange.com/questions/10480/raspi-camera-board-and-motion )
	* sudo modprobe bcm2835-v4l2

## Sensors
https://www.aliexpress.com/item/HOT-16pcs-lot-Raspberry-Pi-3-Raspberry-Pi-2-Model-B-the-sensor-module-package-16/32785335903.html?spm=2114.13010608.0.0.RZVziT

* [DHT11](sensors/DHT11.md) temperature and humidity sensor module 
* HC-SR501 infrared human body induction module
* DS1302 real time clock module
* The rain sensor module
* Sound sensor moduel
* HC-SR04 ultrasonic sensor
* The flame sensor module
* KY-008 laser head sensor module
* Photosensitive resistance sensor module
* The YL-69 soil moisture sensor
* Obstacle avoidance sensor
* Vibration sensor module
* 315M super regenetive module
* The tilt sensor module
* A path tracing module


### Toc Generator
[https://ecotrust-canada.github.io/markdown-toc/](https://ecotrust-canada.github.io/markdown-toc/)



Pogledaj sta je ovo 'tasksel' - kaze da mozes da napravis webserver         
