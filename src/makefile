CC = g++
CFLAGS = -Wall -std=c++1z -g
DEPS = includes.h common.h command_mode.h normal_mode.h
OBJ = common.o command_mode.o normal_mode.o
%.o: %.cpp $(DEPS)
	$(CC) $(CFLAGS) -c -o $@ $<

file_explorer: $(OBJ)
	$(CC) $(CFLAGS) -o $@ $^

clean:
	rm -f *.o file_explorer
