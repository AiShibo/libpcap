PROG= test
SRCS= test.c
CFLAGS += -I${.CURDIR}/../lib/libpcap
CFLAGS += -I${.CURDIR}/../sys
CFLAGS += -I${.CURDIR}/../compat
CFLAGS += -g -O0

LDFLAGS+= -lpcap
LDFLAGS+= -g
LDFLAGS+= -L/home/shibo/libpcap/lib/libpcap

.include <bsd.prog.mk>

run:
	sudo LD_LIBRARY_PATH=/home/shibo/libpcap/lib/libpcap ./test

debug:
	sudo LD_LIBRARY_PATH=/home/shibo/libpcap/lib/libpcap gdb ./test

