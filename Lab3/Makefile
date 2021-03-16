CC = gcc
CFLAGS = -Wall -Wextra -std=c99
SOURCES = main.c
LIBS = -pthread
OBJECTS = $(subst .c, .o, $(SOURCES))
BIN = puzzle
.PHONY: clean help

puzzle: $(OBJECTS)
	$(CC) $(CFLAGS) $^ $(LIBS) -o $@

%.o : %.c
	$(CC) $(CFLAGS) -c $<

all: $(BIN)

clean:
	rm  -f $(OBJECTS) $(BIN) *~