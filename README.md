# mobilesensor

simplesensor for mobile

Made with [Apache Cordova](http://cordova.apache.org/).


To set up cordova's environment correctly : [loopback-users-mobile](https://github.com/BenLeroy/loopback-users-mobile).


Android APK is already built in this [directory](https://github.com/BenLeroy/mobilesensor/blob/master/platforms/android/build/outputs/apk/android-debug.apk).


To make the application point to the right server address, you'll need to change [app.js](https://github.com/BenLeroy/mobilesensor/blob/master/www/js/app.js) :

	- at line 13 (LoopBackResourceProvider); don't forget the '/api' at the end,
	- and line 49 (socket.io connector).


And then rebuild the project's APK with cordova using `$ cordova build` from project's root.


The built APK will be found in [dir]/platforms/android/build/outputs/apk/android-debug.apk .

