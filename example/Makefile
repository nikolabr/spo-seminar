.PHONY
all: libfile.a main.o
	ld libfile.a main.o

main.o: main.c
	gcc -c main.c -o main.o

dir.o: dir.c
	gcc -c dir.c -o dir.o

file.o: file.c
	gcc -c file.c -o file.o

libfile.a: dir.o file.o
	ar rcs libfile.a dir.o file.o
