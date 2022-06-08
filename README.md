
# prerequisites

* Cortex ARM Toolchain, nordic SDK requires:
https://developer.arm.com/tools-and-software/open-source-software/developer-tools/gnu-toolchain/gnu-rm/downloads/9-2019-q4-major

* Nordic SDK nRF5_SDK_17.1.0_ddde560:
https://www.nordicsemi.com/Products/Development-software/nrf5-sdk/download

* Segger JLink:
https://www.segger.com/downloads/jlink/


# setup and build from CLI
       
make a build:

        make -C pca10056/blank/armgcc

# setup and build from vscode

## Required plugins

ms-vscode.cpptools
marus25.cortex-debug
ms-vscode.makefile-tools

## Startup & Build

1.start launcher script:
        
        ./code.sh

2.build: ctrl-p and enter 'task build' or enter ctrl-shift-b

3.clean: 'task clean'

4.debug: enter f5


## detailed integration in VSCode

https://www.novelbits.io/nrf52-visual-studio-code/

Relevant config files:
* c_cpp_properties.json: compiler include path, defines, intellisense,...
* launch.json: debug executable, jlink settings, swd, ....
* tasks.json: mapped to makefile targets, eg build, clean, flash, sdk_config, erase