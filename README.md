# How to build Qt?
## Get ready for Compile Qt5.14.0
```
     sudo apt update
     sudo apt install ssh
     sudo apt install build-essential 
     sudo apt install libgl1-mesa-dev 
     wget http://download.qt.io/official_releases/qt/5.14/5.14.0/single/qt-everywhere-src-5.14.0.tar.xz
     tar xf qt-everywhere-src-5.14.0.tar.xz 
     cd qt-everywhere-src-5.14.0/
     cd ..
     mkdir build
     cd build/
```
## Configure and compile
If you want to install over system:
```
     ../qt-everywhere-src-5.14.0/configure -nomake examples -nomake tests -recheck
     make
     make install
```
If you want to install as another qt for 32 bit machines over 64 bit systems
     ../qt-everywhere-src-5.14.0/configure -nomake examples -nomake tests -recheck -platform linux-g++-32 -prefix $PWD
```  
