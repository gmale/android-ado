# android-ado
### Android Debug Overpass
-----
A utility that leverages Android Debug Bridge to make life a little easier.

For the developer who spends a lot of time on the commandline, ADB can be a bit cumbersome to use. This helps make day-to-day life easier by reducing friction in the following areas for the app that's being developed:

- clearing an app's cache
- deleting an app
- working with multiple devices
  - simultaneous installs
  - simultaneous deletes
  - setting and active device
  - aliases for devices

### Features
#### Defaults
When you install an APK it sets common sense defaults including, the default APK file name, the default package name and the default device.


### Installation Instructions
1. git clone https://github.com/gmale/android-ado.git
2. TODO: complete this list

### Usage Examples
`$ ado -i`    
enters interactive mode, which is great for multiple actions. In this mode, pressing single keys will intiate common actions.

p - set the default package name. auto-complete to select the right one.    
a - set the default APK    
c - clear cache. auto-complete to select the package to clear   
C - clear cache. uses the default package.   
i - install. brings up the list of APKs in the build/outputs/apk folder. From there, type the number of the corresponding APK to install    
I - install the default APK



`$ ado install`    
installs the defualt APK onto the default device




Aliasing
--------
// TODO: reword this language borrowed from Hub (https://github.com/github/hub)

Using ado feels best when it's aliased as `adb`. This is not dangerous; your
_normal adb commands will all work_. ado merely adds some sugar.

`ado alias` displays instructions for the current shell. With the `-s` flag, it
outputs a script suitable for `eval`.

You should place this command in your `.bash_profile` or `.zshrc` or other startup script:

``` sh
eval "$(hub alias -s)"
```
