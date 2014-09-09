#Vector Chart Object Search  Plugin for OpenCPN
This plugin provides a search interface to the objects on the vector charts in OpenCPN. Note that it indexes the objects on the charts which were loaded at least once with the plugin enabled.

##Building
This assumes you have already seen the building instructions at http://opencpn.org/ocpn/compiling_source_linux or http://opencpn.org/ocpn/compiling_source_windows and can build OpenCPN from source.

###Linux:
```
git clone https://github.com/nohal/objsearch_pi.git
cd objsearch_pi
mkdir build
cd build
cmake ..
make
```
###Windows:
You must have opencpn.lib created while OpenCPN application is built in the build folder. If you don't want to make one yourself, there are several prebuilt versions at https://sourceforge.net/projects/opencpnplugins/files/opencpn_lib/ - you need one corresponding to version newer than 3.3.2028
```
git clone https://github.com/nohal/objsearch_pi.git
cd objsearch_pi
mkdir build
```
Copy opencpn.lib into the newly created build folder
```
cd build
cmake ..
cmake --build . --config release
```
