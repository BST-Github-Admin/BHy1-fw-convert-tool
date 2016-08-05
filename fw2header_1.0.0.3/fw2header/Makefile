CC=gcc
CFLAGS=-c -Wall -o2
#LDFLAGS=-lpthread
LDFLAGS=
SOURCES=main.c
OBJECTS=$(SOURCES:.c=.o)
EXECUTABLE=fw2h

all: $(SOURCES) $(EXECUTABLE)

$(EXECUTABLE): $(OBJECTS)
	$(CC) $(OBJECTS) -o $@ $(LDFLAGS)

.c.o:
	$(CC) $(CFLAGS) $< -o $@

clean:
	@rm -rf $(OBJECTS) $(EXECUTABLE)

.PHONY: clean

