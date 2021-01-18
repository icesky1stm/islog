BIN  := \
main_islib_test \

OBJ  += islog_test

LIBS := islog.so

CFLAGS  += -Wall -std=c99 -g -I../src/

LDFLAGS += ../islog.so

.SUFFIXES: .c .so .o

.PHONY: all
all: $(BIN)

.PHONY: $(BIN)
$(BIN): $(OBJ)

.PHONY: clean
clean:
	rm -f *_test *_tmp

%.c:
	$(CC) $(CFLAGS) $(LDFLAGS) $(LIBS) -o $@ $<

