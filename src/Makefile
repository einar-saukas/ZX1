CC = owcc
CFLAGS  = -ox -ob -ol+ -onatx -oh -zp8 -fp6 -g0 -Ot -oe -ot -Wall -xc -s -finline-functions -finline-intrinsics -finline-math -floop-optimize -frerun-optimizer -fno-stack-check -march=i386 -mtune=i686
RM = del
EXTENSION = .exe

all: zx1 dzx1

zx1: zx1.c optimize.c compress.c memory.c zx1.h
	$(CC) $(CFLAGS) -o zx1$(EXTENSION) zx1.c optimize.c compress.c memory.c

dzx1: dzx1.c
	$(CC) $(CFLAGS) -o dzx1$(EXTENSION) dzx1.c

clean:
	$(RM) *.obj
