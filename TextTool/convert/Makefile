all : text

CFLAGS:=-I.. -I.

MINGW32:=/usr/bin/i686-w64-mingw32-

convert.exe : convert.c
	$(MINGW32)gcc -m32 -o $@ $^  -lgdi32 $(CFLAGS)


convert : convert.c
	gcc -o $@ $^ -lm -lpthread -g $(CFLAGS)
	chmod +777 convert
	

clean :
	rm -rf *.o *~ text
	
