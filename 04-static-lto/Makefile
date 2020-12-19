MAINTGT = test-static-lto

.c.o:
	$(CC) -Wall -Wextra -flto -c -O2 $<

$(MAINTGT): test.o aux.o
	$(CC) -Wall -Wextra -static -flto -O2 *.o -o $@

clean:
	rm -rf *.o *~ $(MAINTGT)

.PHONY: clean
