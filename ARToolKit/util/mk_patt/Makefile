INC_DIR= ../../include
LIB_DIR= ../../lib
BIN_DIR= ../../bin

LDFLAG=-L/usr/X11R6/lib -L$(LIB_DIR)
LIBS= -lARgsub_lite -lARvideo -lAR -lglut -lGLU -lGL -lXi -lXmu -lX11 -lm -ljpeg
CFLAG= -O -I/usr/X11R6/include -DUSE_EYETOY -I/usr/src/linux/include -g -I$(INC_DIR)


all: $(BIN_DIR)/mk_patt


$(BIN_DIR)/mk_patt: mk_patt.c
	cc -o $(BIN_DIR)/mk_patt $(CFLAG) mk_patt.c\
	   $(LDFLAG) $(LIBS)

clean:
	rm -f $(BIN_DIR)/mk_patt

allclean:
	rm -f $(BIN_DIR)/mk_patt
	rm -f Makefile
