# setup and build

Setup the environment:    
. ./.env
        
make a build:
make -C pca10056/blank/armgcc

# integration in VSCode

https://www.novelbits.io/nrf52-visual-studio-code/

## Required plugins

ms-vscode.cpptools
marus25.cortex-debug
ms-vscode.makefile-tools

## Startup and confi overview

1.start terminal & read environment vars from file 'env'
        
        source env

2.start vscode

        code .


Build options:

        .vsode/tasks.json

C/C++ config options:

        .vsode/c_cpp_propertioes.json

Debug configuration options:

        .vscode/launch.sh
