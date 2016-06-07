CC=g++
CFLAGS=-W -Wall -ansi -pedantic
LDFLAGS=
EXEC=test

all: $(EXEC)

test: test.o mlp.o
	$(CC) -o test test.o mlp.o $(LDFLAGS)

test.o: mlp.h

%.o: %.cc
	$(CC) -o $@ -c $< $(CFLAGS)

clean:
	rm -rf *.o

mrproper: clean
	rm -rf $(EXEC)

