CC=gcc

all:	../aggcpu.elf ../cpu.elf ../fs.elf

../aggcpu.elf:	aggcpu.c
	$(CC) -o $@ aggcpu.c -lkstat

../cpu.elf:	cpu.c
	$(CC) -o $@ cpu.c -lkstat

../fs.elf:	fs.c
	$(CC) -m64 -D_LARGEFILE64_SOURCE -o $@ fs.c 
