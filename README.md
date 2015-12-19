#React Native Notes

Following this tutorial:
* [http://www.raywenderlich.com/99473/introducing-react-native-building-apps-javascript](http://www.raywenderlich.com/99473/introducing-react-native-building-apps-javascript)

#Installation (OSX)

##Install node >= v4
```
$ brew install nvm
$ nvm ls-remote
$ nvm install v5.3.0    # Or something >=4 
```

The Xcode build process uses the system node which needs to be the >=4, to get this working I added...
```
export NVM_DIR=~/.nvm
source $(brew --prefix nvm)/nvm.sh
```
to the bottom of my ``~/.bash_profile``

##Install XCode
* [https://developer.apple.com/xcode/download/](https://developer.apple.com/xcode/download/)

##Install Watchman and ``react-native-cli``
```
$ brew install watchman
$ npm install -g react-native-cli
```

#Use ``react-native`` CLI to build a basic app
```
$ cd /work # Or where-ever you put your projects
$ react-native init HelloWorld
```

#Open the IOS Project it Xcode
* Open Xcode
* File -> Open ... ``HelloWorld/ios/HelloWorld.xcodeproj``

#Run the App
* BE READY!!! - You may have to very quickly click the ``Allow`` Button before the app crashes
* Click on the ``Run`` icon that looks like a play button
* This should launch app in the simulator and the node server for the backend

#Problems? Things that May Help
* ``brew update``
* ``brew upgrade watchman``

