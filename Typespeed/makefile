CC = g++
CFLAGS = -g -Wall -std=c++11 -fopenmp -lsfml-graphics -lsfml-window -lsfml-system -lsfml-audio
DEPS = header.h Button.hpp MovingBackground.hpp hash.h Settings.hpp
OBJ = main.cpp source.cpp Button.cpp MovingBackground.cpp Settings.cpp

%.o: %.c $(DEPS)
	$(CC) -c -o $@ $< $(CFLAGS)

pa6: $(OBJ)
	$(CC) -o $@ $^ $(CFLAGS)
	
clean:
	-rm *.o
