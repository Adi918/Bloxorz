----------------------------------------------------------------
DEPENDENCIES
----------------------------------------------------------------
Linux/Windows/ Mac OSX - Dependencies: (Recommended)
 GLFW
 GLAD
 GLM

Linux - Dependencies: (alternative)
 FreeGLUT
 GLEW
 GLM

----------------------------------------------------------------
INSTALLATION
----------------------------------------------------------------
GLFW:
 - Install CMake
 - Obtain & Extract the GLFW source code from
   https://github.com/glfw/glfw/archive/master.zip
 - Compile with below commands
   $ cd glfw-master
   $ mkdir build
   $ cd build
   $ cmake -DBUILD_SHARED_LIBS=ON ..
   $ make && sudo make install

GLAD:
 - Go to http://glad.dav1d.de
 - Language: C/C++
   Specification: OpenGL
   gl: Version 4.5
   gles1: Version 1.0
   gles2: Version 3.2
   Profile: Core
   Select 'Add All' under extensions and click Generate.
 - Download the zip file generated.
 - Copy contents of include/ folder in the downloaded directory 
   to /usr/local/include/
 - src/glad.c should be always compiled along with your OpenGL 
   code

GLM:
 - Download the zip file from 
   https://github.com/g-truc/glm/releases/tag/0.9.7.2
 - Unzip it and copy the folder glm/glm/ to /usr/local/include

Ubuntu users can also install these libraries using apt-get.
It is recommended to use GLFW+GLAD+GLM on all OSes.


FreeGLUT+GLEW+GLM can be used only on linux but not recommended.
Use apt-get to install FreeGLUT, libglew, glm on Linux.
