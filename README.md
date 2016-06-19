Jasper-Module-Selfie
======================

Jasper Selfie Module for my [HAL9000 Raspberry PI Instructable](http://www.instructables.com/id/RaspberryPI-HAL9000/)

##Steps to install Selfie Module

* Install the `fswebcam` package:
```
sudo apt-get install fswebcam
```
* run the following commands in order:
```
git clone https://github.com/ArtBIT/jasper-module-selfie.git
cp jasper-module-selfie/Selfie.py <path to jasper/client/modules>
cp jasper-module-selfie/shutter.wav ~/
#i.e. cp jasper-module-selfie/Selfie.py /usr/local/lib/jasper/client/modules/
```
* Edit `~/.jasper/profile.yml` and add the follwing at the bottom:
```
selfie:
  email: 'email.to.send.pictures@whatever.com'
```
* Make sure you have [mailgun](http://jasperproject.github.io/documentation/configuration/#mailgun) or gmail account set-up for Jasper.
* Restart the Pi:
```
sudo reboot
```
##Congrats, JASPER Selfie Module is now installed and ready for use.
Here are some examples:
```
YOU: Take a photo.
JASPER: *shutter sound* Nice.
YOU: Selfie.
JASPER: *shutter sound* Cute.
```

##Credits
[shutter.wav](https://www.freesound.org/people/benjohansen/sounds/87149/) was sampled by Ben Johansen 
