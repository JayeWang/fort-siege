# Compilation instruction on different compilers
## Codeblocks and Visual Studios
----------------------------------------------------------------------------------------------------------------
1. First we create Character static library:
Create a new project -> choose static library
Add in Character.h and Character.cpp (be sure to link them in the project property settings).
Build the library.
2. Then go ahead and create a new empty project, include all the .cpp and .h files, and also the newly made Character library. Then compile normally.
## Mac terminal/Linux
-----------------------------------------------------------------------------------------------------------------
1. First we create Character static library by using these commands:
- g++ -Wall -std=c++11 -c Character.cpp
- ar r libcharacter.a Character.o
- g++ -Wall -std=c++11 Area.cpp CheatEngine.cpp Room.cpp RoomDescription.cpp main.cpp -L. -lcharacter
2. Then go ahead and include all the .cpp and .h files, and also the newly made Character library and compile normally.
