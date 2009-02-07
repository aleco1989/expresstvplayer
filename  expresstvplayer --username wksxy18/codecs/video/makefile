AVC_TATGET=libavc.so

ALL_OBJECTS=h264.o h264_parser.o bitstream.o  golomb.o #dsputil.o \
            #simple_idct.o

all:$(AVC_TATGET)

$(AVC_TATGET):$(ALL_OBJECTS)
	@gcc $(CFLAGS) -o $@  $^
$(ALL_OBJECTS):$(ALL_OBJECTS:%.o=%.c)
	@gcc -c $^
clean:
	@rm *.o
	@rm $(AVC_TATGET)
help:
	@echo "test!"
