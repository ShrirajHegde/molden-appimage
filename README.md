# Molden Appimage

Molden 6.7 Appimage and build instructions

## Building molden

### Install build dependencies:

in debian/ubuntu:

     sudo apt install gfortran  libx11-6 libx11-dev libgl1-mesa-glx libgl1-mesa-dev build-essential mesa-common-dev libglu1-mesa-dev libxmu-dev xutils-dev wget

refer this for more detail / other distros https://www3.cmbi.umcn.nl/molden/linux.html

* go to build-molden directory
* extract molden6.7.tar.gz
* `cd molden6.7`
* make
* find output binaries in `molden6.7/bin`, you can use them directly

## Creating appimage

* copy files in `molden6.7/bin` to `create-appimage/molden-bin`
* open terminal in `create-appimage`directory
* execute `./pkg2appimage-1803-x86_64.AppImage molden.yml`

* find appimage in `out` directory, test with `./Molden-.glibc2.29-x86_64.AppImage ../test.pdb`
