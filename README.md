# CMake for the IDA Pro SDK

This project provides CMake support for building IDA Pro modules.

## Usage

First, you need to somehow get a copy of this project as a subdirectory
of your project named `external/cmake-microchip`. If you use git, the
easiest way is to add a submodule:

    git submodule add git://github.com/Elemecca/cmake-ida.git external/cmake-ida

Then add this snippet near the top of your `CMakeLists.txt` (after the
`project` command, but before any targets):

    list(APPEND CMAKE_MODULE_PATH external/cmake-ida)
    find_package(IDA 7.0 REQUIRED)



## Copying

Copyright 2017 Sam Hanes.

This project is provided under the same BSD 3-Clause license as CMake
itself. See `COPYING.txt` for details.
