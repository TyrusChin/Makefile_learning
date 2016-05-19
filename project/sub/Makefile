OBJS = sub_int.o sub_float.o

all:$(OBJS)
$(OBJS):%o:%c
	$(CC) -o $(OBJSDIR)/$@ -c $< -O2

clean:
	-$(RM) $(OBJS)

