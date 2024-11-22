CSAPP_DIR = ../../csapp_lib
CSAPP_SRC = $(CSAPP_DIR)/csapp.c
CSAPP_INC = $(CSAPP_DIR)

# Compiler settings
CC = gcc
CFLAGS = -g -Wall -I$(CSAPP_INC)

# Target
TARGET = main

# Build rules
all: $(TARGET)

$(TARGET): main.o
	$(CC) $(CFLAGS) -o $@ $^ $(CSAPP_SRC)

main.o: main.c
	$(CC) $(CFLAGS) -c main.c

clean:
	rm -f $(TARGET) *.o
