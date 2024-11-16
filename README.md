# Interactive-Shape-Modelling

1. brew install freeglut
2. brew list freeglut
3. g++ surfaceModeller.cpp -o a2 -DGL_SILENCE_DEPRECATION \
-I/opt/homebrew/Cellar/freeglut/<version>/include \
-L/opt/homebrew/Cellar/freeglut/<version>/lib \
-framework OpenGL -lglut
