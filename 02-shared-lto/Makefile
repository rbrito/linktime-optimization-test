MAINTGT = test-shared-lto

.c.o:
	$(CC) -Wall -Wextra -c -O2 -flto $<

$(MAINTGT): test.o aux.o
	$(CC) -Wall -Wextra -O2 *.o -flto -o $@

clean:
	rm -rf *.o *~ $(MAINTGT)

.PHONY: clean
