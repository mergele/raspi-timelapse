# raspi-timelapse
Setup a raspberry pi for timelapse photography with a Canon EOS 50D

# initial setup
download and install raspbian jessie lite from https://www.raspberrypi.org/downloads/raspbian/

```bash
raspi-config
# memory split
# enable ssh
# expand filesystem
# change locale and wifi-settings to german / utf8
# change timezone to europe-berlin
```

change password for pi
change password for root

apt update && apt upgrade -y

## basic setup
```bash
apt install vim-tiny mc tmux
apt install dnsutils
apt install postfix
apt install alpine
```

### dyndns
adduser keksdns for dyndns

# problem: 1 malig ohne script ausführen, dann wird der key-auth-mechanismus mit abfrage einmal ausgeführt
# problem: dig braucht einen nameserver, der die angefragte domaine auch kennt, @8.8.8.8 hat funktioniert.


### gphoto2
# Problem: bei raspbian jessie enthaltenes gphoto2 funktioniert nicht, deshalb Installation aus sourcen 
# Problem: Pfad zu gphoto2 wird von CRON nicht erkannt

# inspiration


### INSPIRATION ###
* [http://blog.davidsingleton.org/raspberry-pi-timelapse-controller/]
* [http://www.makeuseof.com/tag/how-to-capture-time-lapse-photography-with-your-raspberry-pi-and-dslr-or-usb-webcam/]


* https://github.com/gonzalo/gphoto2-updater/releases

http://gphoto.org/doc/manual/ref-gphoto2-cli.html
http://gphoto.org/doc/manual/using-gphoto2.html
https://www.neowin.net/forum/topic/142188-gphoto2/
https://www.google.de/search?q=gphoto2+format+card&oq=gphoto2+format+card&aqs=chrome..69i64j5l2.9736j0j7&sourceid=chrome&ie=UTF-8
http://www.gphoto.org/doc/manual/ref-gphoto2-cli.html
http://www.gphoto.org/doc/manual/ref-gphoto2-cli.html#cli-examples
http://www.gphoto.org/doc/manual/using-gphoto2.html
http://www.gphoto.org/doc/remote/
https://github.com/gphoto/gphoto2/issues/20
