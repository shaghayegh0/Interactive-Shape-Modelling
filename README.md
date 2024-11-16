# Interactive-Shape-Modelling

## how to compile and run on macOS
1. brew install freeglut
2. brew list freeglut
3. brew install --cask xquartz
4. open -a XQuartz
5. export DISPLAY=:0
6.  g++ surfaceModeller.cpp -o a2 -DGL_SILENCE_DEPRECATION \
-I/opt/homebrew/Cellar/freeglut/3.6.0/include \
-I/opt/homebrew/Cellar/glew/2.2.0_1/include \
-L/opt/homebrew/Cellar/freeglut/3.6.0/lib \
-L/opt/homebrew/Cellar/glew/2.2.0_1/lib \
-framework OpenGL -lglut -lGLEW -g
7. lldb ./a2 => run

## headers for macOS
- #include <GL/freeglut.h>
- #include <math.h>
- #include <string.h>
- #include "surfaceModeller.h"
- #include "subdivcurve.h"
- #include <OpenGL/gl.h>
- #include <OpenGL/glu.h>
