IOP_BIN  = ds3ps2.irx
IOP_OBJS = ds3ps2.o exports.o imports.o

IOP_CFLAGS += -Wall -fno-builtin-printf -fno-builtin-memcpy

all: $(IOP_BIN)

clean:
	rm -f -r $(IOP_OBJS) $(IOP_BIN)

install: $(IOP_BIN)
	cp $(IOP_BIN) $(PS2SDK)/iop/irx
	cp ds3ps2.h   $(PS2SDK)/iop/include
	cp ds3ps2.h   $(PS2SDK)/ee/include

#FOR ME!!
copy: $(IOP_BIN)
	cp $(IOP_BIN) /media/$(USER)/MLG
	sync

include $(PS2SDK)/samples/Makefile.pref
include $(PS2SDK)/samples/Makefile.iopglobal
