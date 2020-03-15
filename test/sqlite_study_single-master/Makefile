a.out: sqlite3.o test1.o
	gcc -g sqlite3.o test1.o -o a.out -lpthread -ldl

sqlite3.o:sqlite3.c
	gcc -g -c sqlite3.c

test1.o:test1.c
	gcc -g -c test1.c

clean:
	rm -rf test1.o sqlite3.o a.out test.db
