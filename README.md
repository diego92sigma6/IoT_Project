# Development setup
There are a couple of steps to follow in order to debug this program

1. Install VSCode
2. Install [OpenOCD](http://www.freddiechopin.info/en/download/category/4-openocd)
2. 1. Change .vscode/launch.json->windows->debugServerPath to the location of openocd.exe
2. 2. Modify args as needed
3. Install [GNU Arm Embedded Toolchain](https://developer.arm.com/tools-and-software/open-source-software/developer-tools/gnu-toolchain/gnu-rm/downloads)
3. 1. Change .vscode/launch.json->windows->MIDebuggerPath to point to the right location of arm-none-eabi-gdb.exe
4. Make sure to install either MinGW or Cygwin, which contain binaries for C++ and C programming (gdb, g++, etc). Note that this is required since it launches tasks such as make.exe, etc.
5. Done. Start debugging!