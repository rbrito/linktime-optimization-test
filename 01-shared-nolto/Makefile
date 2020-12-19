MAINTGT = test-shared-nolto

.c.o:
	$(CC) -Wall -Wextra -c -O2 $<

$(MAINTGT): test.o aux.o
	$(CC) -Wall -Wextra -O2 *.o -o $@

clean:
	rm -rf *.o *~ $(MAINTGT)

.PHONY: clean
