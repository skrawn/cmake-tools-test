Wherever you clone this, set cmake.cmakePath to an absolute path. This variable doesn't seem to be able to use ${workspaceRoot}.

Build Output:

```
[proc] Executing command: /home/sdonohue/Documents/GitHub/cmake-tools-test/usr/bin/cmake --no-warn-unused-cli -DCMAKE_C_COMPILER:FILEPATH=arm-poky-linux-gnueabi-gcc -DCMAKE_CXX_COMPILER:FILEPATH=arm-poky-linux-gnueabi-g++ -DCMAKE_EXPORT_COMPILE_COMMANDS:BOOL=TRUE -DCMAKE_BUILD_TYPE:STRING=Debug -H/home/sdonohue/Documents/GitHub/cmake-tools-test -B/home/sdonohue/Documents/GitHub/cmake-tools-test/build
[cmake] Not searching for unused variables given on the command line.
[cmake] -- The C compiler identification is unknown
[cmake] -- The CXX compiler identification is unknown
[cmake] CMake Error at CMakeLists.txt:3 (PROJECT):
[cmake]   The CMAKE_C_COMPILER:
[cmake] 
[cmake]     arm-poky-linux-gnueabi-gcc
[cmake] 
[cmake]   is not a full path and was not found in the PATH.
[cmake] 
[cmake]   Tell CMake where to find the compiler by setting either the environment
[cmake]   variable "CC" or the CMake cache entry CMAKE_C_COMPILER to the full path to
[cmake]   the compiler, or to the compiler name if it is in the PATH.
[cmake] 
[cmake] 
[cmake] CMake Error at CMakeLists.txt:3 (PROJECT):
[cmake]   The CMAKE_CXX_COMPILER:
[cmake] 
[cmake]     arm-poky-linux-gnueabi-g++
[cmake] 
[cmake]   is not a full path and was not found in the PATH.
[cmake] 
[cmake]   Tell CMake where to find the compiler by setting either the environment
[cmake]   variable "CXX" or the CMake cache entry CMAKE_CXX_COMPILER to the full path
[cmake]   to the compiler, or to the compiler name if it is in the PATH.
[cmake] 
[cmake] 
[cmake] -- Configuring incomplete, errors occurred!
[cmake] See also "/home/sdonohue/Documents/GitHub/cmake-tools-test/build/CMakeFiles/CMakeOutput.log".
[cmake] See also "/home/sdonohue/Documents/GitHub/cmake-tools-test/build/CMakeFiles/CMakeError.log".
```

With cmake.useCmakeServer: true:

```
[cmake] CMake Error: CMake was unable to find a build program corresponding to "Unix Makefiles".  CMAKE_MAKE_PROGRAM is not set.  You probably need to select a different build tool.
[cmake] Configuring incomplete, errors occurred!
[cms-driver] Error during CMake configure: [cmake-server] Configuration failed.
```