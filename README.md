Android Misc Tools
==================

Initial Base Repository : https://github.com/jakev/android-tools

However now this is used as a collection repository for all single file misc tools that we can find.

For any questions contact anant[@]anantshri[.]info

--------------
INDEX OF FILES WITH SOURCES
--------------

* apkget : https://github.com/jakev/android-tools
* getimage.sh : https://github.com/jakev/android-tools
* sendsecretcode : https://github.com/jakev/android-tools
* /binaries/* : https://github.com/jakev/android-binaries


---------------------------------
OLD README

-----------------------------------

About
-----
A collection of tools and utils to help with Android application assessments and forensics.  Please report issues to javallet[at]gmail[dot]com.

getimage.sh
-----------
A shell script to create and pull a new "system.img" file for an emulator.  Requires the Android SDK, root privileges on the emulator, and enough space to hold the image in the new system.img file. 

apkget
------
A shell script to search for APK files on a device or emulator, and pull them down by package name.

**Usage:**

Searching for a package containg the string "jake":

	root@analysis# ./apkget -s jake
	
Pulling a package off of a physical device:

	root@anaylsis# ./apkget -d -p com.jakev.testing

sendsecretcode
--------------
A shell script to make it easier to send SECRET_CODE intents.

sending the SECRET_CODE intent with the host "jakesecret":

	root@analysis# ./sendsecretcode jakesecret
