CC = gcc
BIN = server.exe
OBJ = client.o conditions.o game.o server.o

all: $(BIN) move

$(BIN): $(OBJ)
	$(CC) $^ -o $@ -lpthread

%.o: %.c
	$(CC) -c $< -o $@

move: 
	mv server.exe ../
	mv *.o ../c_bin/
