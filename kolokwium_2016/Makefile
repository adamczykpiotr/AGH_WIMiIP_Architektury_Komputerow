CC=g++
CFLAGS=-c
ASM=nasm
AFLAGS=-f elf64
#OPT=-O2

FILENAME1 = main
FILENAME2 = zad3


app: $(FILENAME1).o $(FILENAME2).o
	$(CC) $(OPT) $(FILENAME1).o $(FILENAME2).o -o $(FILENAME2)


$(FILENAME1).o: $(FILENAME1).cpp
	$(CC) $(CFLAGS) $(OPT) $(FILENAME1).cpp


$(FILENAME2).o: $(FILENAME2).asm
	$(ASM)  $(AFLAGS) $(FILENAME2).asm

clean:
	rm -f *.o
