CC=cc
CFLAGS=-g -ansi -std=gnu99 -Wall

BINS=insertion merge quick counting comparison heaparray
all: $(BINS)

# O(n) Sorting:
insertion: %:%.c
	$(CC) $(CFLAGS) $^ -o $@
comparison: %:%.c
	$(CC) $(CFLAGS) $^ -o $@

# O(n log n); Divide and Conquer:
heaparray: %:%.c
	$(CC) $(CFLAGS) $^ -o $@
merge: %:%.c
	$(CC) $(CFLAGS) $^ -o $@
quick: %:%.c
	$(CC) $(CFLAGS) $^ -o $@

# Non Comparison Sorting:
counting: %:%.c
	$(CC) $(CFLAGS) $^ -o $@

.PHONY: clean
clean:
	@- $(RM) $(BINS)
