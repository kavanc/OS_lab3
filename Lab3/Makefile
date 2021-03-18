CC = gcc
CFLAGS = -Wall -Wextra -std=c99
SOURCES = main.c
LIBS = -pthread
BIN = puzzle
.PHONY: clean help

puzzle: main.c
	$(CC) $(CFLAGS) $^ $(LIBS) -o $@

%.o : %.c
	$(CC) $(CFLAGS) -c $<

all: $(BIN)

clean:
	rm  -f $(OBJECTS) $(BIN) *~