#CC = cc
CC = gcc

CFLAGS= -O3 -Wall

all: mkdskimg bin2hex send receive ptp2bin
	@echo
	@echo "Done."
	@echo

mkdskimg: mkdskimg.c
	$(CC) $(CFLAGS) -o mkdskimg mkdskimg.c
	cp mkdskimg ${HOME}/bin

bin2hex: bin2hex.c
	$(CC) $(CFLAGS) -o bin2hex bin2hex.c
	cp bin2hex ${HOME}/bin 

send: send.c
	$(CC) $(CFLAGS) -o send send.c
	cp send ${HOME}/bin

receive: receive.c
	$(CC) $(CFLAGS) -o receive receive.c
	cp receive ${HOME}/bin

ptp2bin: ptp2bin.c
	$(CC) $(CFLAGS) -o ptp2bin ptp2bin.c
	cp ptp2bin ${HOME}/bin

clean:
	rm -f mkdskimg mkdskimg.exe bin2hex bin2hex.exe receive receive.exe \
	send send.exe ptp2bin ptp2bin.exe
