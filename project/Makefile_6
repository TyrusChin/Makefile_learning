CC = gcc
CFLAGS = -Iadd -Isub -O2
TARGET = cacu7
DIR = add sub .

FILES = $(foreach dir, $(DIR), $(wildcard $(dir)/*.c) )
OBJS = $(patsubst %c, %o, $(FILES))

$(TARGET):$(OBJS) main.o
	$(CC) -o $@ $^ -O2

$(OBJS):%o:%c
	$(CC) -o $@ -c $< $(CFLAGS)

clean:
	-$(RM) $(TARGET) $(OBJS)
