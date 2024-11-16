# Interactive-Shape-Modelling

## how to compile and run on macOS
1. brew install freeglut
2. brew list freeglut
3. brew install --cask xquartz
4. open -a XQuartz
5. export DISPLAY=:0
6. g++ surfaceModeller.cpp -o a2 -DGL_SILENCE_DEPRECATION \
-I/opt/homebrew/Cellar/freeglut/<version>/include \
-L/opt/homebrew/Cellar/freeglut/<version>/lib \
-framework OpenGL -lglut
7. ./a2

## headers for macOS
- #include <GL/freeglut.h>
- #include <math.h>
- #include <string.h>
- #include "surfaceModeller.h"
- #include "subdivcurve.h"
- #include <OpenGL/gl.h>
- #include <OpenGL/glu.h>
