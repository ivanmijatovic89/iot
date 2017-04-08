# iot Basic
Table of content:
* [Commands](#AutoLogin the Raspbian)
* VNC VIEWER (remote connection)
* AutoLogin ( start process when pi boot )

## Commands
| command       | Description |
| ------------- |:-------------:|
| startx      	| start desktop GUI |


## VNC VIEWER on Mac osx:

	https://smittytone.wordpress.com/2016/03/02/mac_remote_desktop_pi/
	
	sudo apt-get install tightvncserver
	
	tightvncserver
	
	# to set resolution :
	# tightvncserver -geometry 1920x1080 -depth 24

	# connect using VNC VIEWER to:
	vnc://pi.local:1

## AutoLogin the Raspbian
	
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


Pogledaj sta je ovo 'tasksel' - kaze da mozes da napravis webserver         
