# Interactive-Shape-Modelling

## how to compile and run on macOS
1. brew install freeglut
2. brew list freeglut
3. brew install glew
4. brew install --cask xquartz
5. open -a XQuartz
6. export DISPLAY=:0
7. g++ surfaceModeller.cpp -o a2 \
-I/opt/homebrew/Cellar/freeglut/3.6.0/include \
-I/opt/homebrew/Cellar/glew/2.2.0_1/include \
-L/opt/homebrew/Cellar/freeglut/3.6.0/lib \
-L/opt/homebrew/Cellar/glew/2.2.0_1/lib \
-framework OpenGL -lglut -lGLEW
8. ./a2

## headers for macOS
#define GL_SILENCE_DEPRECATION
#include <GL/freeglut.h>
#include <math.h>
#include <string.h>
#include "surfaceModeller.h"
#include "subdivcurve.h"
#include <OpenGL/gl.h>
#include <OpenGL/glu.h>
#include <unistd.h>
#include <stdio.h>

