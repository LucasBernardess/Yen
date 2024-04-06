CC = gcc
CFLAGS = -Wall -Wextra -g
INCLUDES = -Iinclude

SRC_DIR = src
OBJ_DIR = obj

all: main

main: $(OBJ_DIR)/main.o $(OBJ_DIR)/file_io.o $(OBJ_DIR)/graph.o $(OBJ_DIR)/dijkstra.o $(OBJ_DIR)/yen.o $(OBJ_DIR)/paths.o
	$(CC) $(CFLAGS) $(INCLUDES) -o main $(OBJ_DIR)/main.o $(OBJ_DIR)/file_io.o $(OBJ_DIR)/graph.o $(OBJ_DIR)/dijkstra.o $(OBJ_DIR)/yen.o $(OBJ_DIR)/paths.o

$(OBJ_DIR)/main.o: $(SRC_DIR)/main.c include/file_io.h include/graph.h include/dijkstra.h include/yen.h include/paths.h
	$(CC) $(CFLAGS) $(INCLUDES) -c $(SRC_DIR)/main.c -o $(OBJ_DIR)/main.o

$(OBJ_DIR)/file_io.o: $(SRC_DIR)/file_io.c include/file_io.h include/graph.h include/dijkstra.h include/yen.h include/paths.h
	$(CC) $(CFLAGS) $(INCLUDES) -c $(SRC_DIR)/file_io.c -o $(OBJ_DIR)/file_io.o

$(OBJ_DIR)/graph.o: $(SRC_DIR)/graph.c include/graph.h
	$(CC) $(CFLAGS) $(INCLUDES) -c $(SRC_DIR)/graph.c -o $(OBJ_DIR)/graph.o

$(OBJ_DIR)/dijkstra.o: $(SRC_DIR)/dijkstra.c include/dijkstra.h
	$(CC) $(CFLAGS) $(INCLUDES) -c $(SRC_DIR)/dijkstra.c -o $(OBJ_DIR)/dijkstra.o

$(OBJ_DIR)/yen.o: $(SRC_DIR)/yen.c include/yen.h include/dijkstra.h include/graph.h
	$(CC) $(CFLAGS) $(INCLUDES) -c $(SRC_DIR)/yen.c -o $(OBJ_DIR)/yen.o

$(OBJ_DIR)/paths.o: $(SRC_DIR)/paths.c include/paths.h
	$(CC) $(CFLAGS) $(INCLUDES) -c $(SRC_DIR)/paths.c -o $(OBJ_DIR)/paths.o

clean:
	rm -f main $(OBJ_DIR)/*.o
