Qt install Tutorial for Comp 406 Project 2
===
**Authors: Nick Young**

**Date: 2024-03-11**

# The gist

There are two different ways this tutorial is going to discuss using Qt.

1. Qt creator
2. Qmake

I'm going to describe it for two platforms--Linux, and Windows. The steps for Windows and MacOS should be fairly similar but I haven't tested them yet.

# Linux

This part of the tutorial will assume you are using a Linux Mint Virtual Machine to install and use software. Version should not matter.

## Dependencies

These are the dependencies that should be needed for qt creator and qmake. Run this command and you should be good to go.

	sudo apt install qtbase5-dev qtbase5-dev-tools 

I pulled these from a [stackoverflow question](https://askubuntu.com/questions/1365515/how-to-install-qmake-compiler-on-ubuntu). If there are missing dependencies, look here first.

## Qt creator

### Steps to install

To install the open source verion of Qt creator, do not go to the Qt website. Open a terminal and type 

	sudo apt install qtcreator

This will download and install Qt creator.

### Steps to use

Open Qt creator either through the terminal or the application menu.

To open Project 2, download ALL of the files from the blackboard and keep them in the same directory.

Create your gameboy.cpp file in the same directory.

After the "Projects" header, click "Open" and open the gameboy.pro file. This is a project file which understands what files are needed to be opened, and Qt creator will automatically open the header files and the source files.

CONGRATS. You now have an open source installation of Qt creator.

## Qmake

Run

	sudo apt install qt5-make

Run 

    qmake

in the directory with all your files. You should only need to do this when you update the headers of your gameboy.cpp file.

Every time you want to compile from now on, run

	make

in the directory with all your files.

CONGRATS. You now have qmake and don't have to screw around with Qt creator.

# Windows

Make sure you don't have Visual Studio or VSCode installed.

## Qt creator

Download the 5.12.x offline installer from [qt.io/offline-installers](https://www.qt.io/offline-installers)

Turn off your wifi. Otherwise you need to make and use an account.

### Installation folder

Accept the default installation folder.

### Select Components Step

Under the Qt 5.12.x dropdown, select MinGW 7.30 64-bit

Under the Developer and Designer Tools dropdown, select Qt Creator 5.0.2 CDB Debugger Support and MinGW 7.3.0 64-bit

### License Agreement

Agree.

### Start Menu shortcuts

Click next.

### Ready to Install

Click next.

### Finished

From here, follow the "Steps to use" section below.

### Steps to use

Open Qt Creator.

To open Project 2, download ALL of the files from the blackboard and keep them in the same directory.

Create your gameboy.cpp file in the same directory.

After the "Projects" header, click "Open" and open the gameboy.pro file. This is a project file which understands what files are needed to be opened, and Qt creator will automatically open the header files and the source files.

CONGRATS. You now have an open source installation of Qt creator.

## Qmake

Qmake is installed alongside Qt Creator with the listed steps above.

Now to add qmake to your path, follow [this tutorial on medium](https://medium.com/@kevinmarkvi/how-to-add-executables-to-your-path-in-windows-5ffa4ce61a53) assuming the path for qmake is something like C:Qt\\Qt5.12.x\\mingw73_64\\bin\\qmake

Run 

    qmake

in the directory with all your files. You should only need to do this when you update the headers of your gameboy.cpp file.

Every time you want to compile from now on, run

	make

in the directory with all your files.

CONGRATS. You now have qmake and don't have to screw around with Qt creator.

