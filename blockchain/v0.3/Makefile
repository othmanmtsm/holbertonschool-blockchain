C = gcc
CFLAGS = -Wall -Werror -Wextra -pedantic -I. -Itransaction -Iprovided -I../../crypto
AR = ar -rcs
RM = rm -f
CTAGS = ctags
TAGS = .tags

TASK0 = blockchain_create
TASK1 = block_create
TASK2 = block_destroy
TASK3 = blockchain_destroy
TASK4 = block_hash
TASK5 = blockchain_serialize
TASK6 = blockchain_deserialize
TASK7 = block_is_valid
TASK10 = hash_matches_difficulty
TASK11 = block_mine
TASK12 = blockchain_difficulty
TASK13 = tx_out_create
TASK14 = unspent_tx_out_create
TASK15 = tx_in_create
TASK16 = transaction_hash
TASK17 = tx_in_sign
TASK17 = tx_in_sign
TASK18 = transaction_create
TASK19 = transaction_is_valid
TASK20 = coinbase_create
TASK21 = coinbase_is_valid
TASK22 = transaction_destroy

SRC = $(wildcard *.c) $(wildcard transaction/*.c) $(wildcard provided/*.c)
OBJ = $(patsubst %.c,%.o,$(SRC))

$(TASK22): transaction/$(TASK22).c transaction/$(TASK21).c transaction/$(TASK20).c transaction/$(TASK18).c transaction/$(TASK17).c transaction/$(TASK16).c transaction/$(TASK15).c transaction/$(TASK14).c transaction/$(TASK13).c transaction/test/$(TASK22)-main.c provided/_print_hex_buffer.c provided/_transaction_print.c
	$(CC) $(CFLAGS) -o $@  $^ $(LIBS)
$(TASK21): transaction/$(TASK21).c transaction/$(TASK20).c transaction/$(TASK18).c transaction/$(TASK17).c transaction/$(TASK16).c transaction/$(TASK15).c transaction/$(TASK14).c transaction/$(TASK13).c transaction/test/$(TASK21)-main.c provided/_print_hex_buffer.c provided/_transaction_print.c
	$(CC) $(CFLAGS) -o $@  $^ $(LIBS)

$(TASK20): transaction/$(TASK20).c transaction/$(TASK18).c transaction/$(TASK17).c transaction/$(TASK16).c transaction/$(TASK15).c transaction/$(TASK14).c transaction/$(TASK13).c transaction/test/$(TASK20)-main.c provided/_print_hex_buffer.c provided/_transaction_print.c
	$(CC) $(CFLAGS) -o $@  $^ $(LIBS)

$(TASK19): transaction/$(TASK19).c transaction/$(TASK18).c transaction/$(TASK17).c transaction/$(TASK16).c transaction/$(TASK15).c transaction/$(TASK14).c transaction/$(TASK13).c transaction/test/$(TASK19)-main.c provided/_print_hex_buffer.c provided/_transaction_print.c
	$(CC) $(CFLAGS) -o $@  $^ $(LIBS)

$(TASK18): transaction/$(TASK18).c transaction/$(TASK17).c transaction/$(TASK16).c transaction/$(TASK15).c transaction/$(TASK14).c transaction/$(TASK13).c transaction/test/$(TASK18)-main.c provided/_print_hex_buffer.c provided/_transaction_print.c
	$(CC) $(CFLAGS) -o $@  $^ $(LIBS)

$(TASK17): transaction/$(TASK17).c transaction/$(TASK16).c transaction/$(TASK15).c transaction/$(TASK14).c transaction/$(TASK13).c transaction/test/$(TASK17)-main.c provided/_print_hex_buffer.c provided/_transaction_print.c
	$(CC) $(CFLAGS) -o $@  $^ $(LIBS)

$(TASK16): transaction/$(TASK16).c transaction/$(TASK15).c transaction/$(TASK14).c transaction/$(TASK13).c transaction/test/$(TASK16)-main.c provided/_print_hex_buffer.c provided/_transaction_print.c
	$(CC) $(CFLAGS) -o $@  $^ $(LIBS)

$(TASK15): transaction/$(TASK15).c transaction/$(TASK14).c transaction/$(TASK13).c transaction/test/$(TASK15)-main.c provided/_print_hex_buffer.c
	$(CC) $(CFLAGS) -o $@  $^ $(LIBS)

$(TASK14): transaction/$(TASK14).c transaction/$(TASK13).c transaction/test/$(TASK14)-main.c provided/_print_hex_buffer.c
	$(CC) $(CFLAGS) -o $@  $^ $(LIBS)

$(TASK13): transaction/$(TASK13).c transaction/test/$(TASK13)-main.c provided/_print_hex_buffer.c
	$(CC) $(CFLAGS) -o $@  $^ $(LIBS)

$(TASK12): $(TASK12).c test/$(TASK12)-main.c $(TASK11).c $(TASK10).c $(TASK7).c $(TASK4).c $(TASK3).c $(TASK2).c $(TASK1).c $(TASK0).c $(PROVIDED)
	$(CC) $(CFLAGS) -o $@  $^ $(LIBS)

$(TASK11): $(TASK11).c test/$(TASK11)-main.c $(TASK10).c $(TASK7).c $(TASK4).c $(TASK3).c $(TASK2).c $(TASK1).c $(TASK0).c $(PROVIDED)
	$(CC) $(CFLAGS) -o $@  $^ $(LIBS)

$(TASK10): $(TASK10).c test/$(TASK10)-main.c
	$(CC) $(CFLAGS) -o $@  $^ $(LIBS)

$(TASK7): $(TASK7).c $(TASK6).c $(TASK5).c $(TASK4).c $(TASK3).c $(TASK2).c $(TASK1).c $(TASK0).c test/$(TASK7)-main.c $(PROVIDED)
	$(CC) $(CFLAGS) -o $@  $^ $(LIBS)

$(TASK6): $(TASK6).c $(TASK5).c $(TASK4).c $(TASK3).c $(TASK2).c $(TASK1).c $(TASK0).c test/$(TASK6)-main.c $(PROVIDED)
	$(CC) $(CFLAGS) -o $@  $^ $(LIBS)

$(TASK5): $(TASK5).c $(TASK4).c $(TASK3).c $(TASK2).c $(TASK1).c $(TASK0).c test/$(TASK5)-main.c $(PROVIDED)
	$(CC) $(CFLAGS) -o $@  $^ $(LIBS)

$(TASK4): $(TASK4).c $(TASK3).c $(TASK2).c $(TASK1).c $(TASK0).c test/$(TASK4)-main.c provided/_blockchain_print.c provided/_blockchain_destroy.c transaction/$(TASK22).c transaction/$(TASK21).c transaction/$(TASK20).c transaction/$(TASK18).c transaction/$(TASK17).c transaction/$(TASK16).c transaction/$(TASK15).c transaction/$(TASK14).c transaction/$(TASK13).c transaction/test/$(TASK22)-main.c provided/_print_hex_buffer.c provided/_transaction_print.c
	$(CC) $(CFLAGS) -o $@  $^ $(LIBS)

$(TASK3): $(TASK3).c $(TASK2).c $(TASK1).c $(TASK0).c test/$(TASK3)-main.c provided/_blockchain_print.c provided/_blockchain_destroy.c
	$(CC) $(CFLAGS) -o $@  $^ $(LIBS)

$(TASK2): $(TASK2).c $(TASK1).c $(TASK0).c test/$(TASK2)-main.c provided/_blockchain_print.c provided/_blockchain_destroy.c provided/_print_hex_buffer.c provided/_transaction_print.c provided/_transaction_print_brief.c
	$(CC) $(CFLAGS) -o $@  $^ $(LIBS)

$(TASK1): $(TASK1).c $(TASK2).c  $(TASK0).c test/block_create-main.c provided/_blockchain_print.c blockchain_destroy.c provided/_print_hex_buffer.c provided/_transaction_print.c provided/_transaction_print_brief.c transaction/transaction_destroy.c
	$(CC) $(CFLAGS) -o $@  $^ $(LIBS)

$(TASK0): $(TASK0).c test/blockchain_create-main.c provided/_blockchain_print.c provided/_blockchain_destroy.c
	$(CC) $(CFLAGS) -o $@  $^ $(LIBS)

.PHONY: all clean distclean oclean tags libhblk_blockchain.a

all: libhblk_blockchain.a

clean: oclean
	$(RM) libhblk_crypto.a

distclean: clean
	$(RM) $(TAGS)

oclean:
	$(RM) $(OBJ)

tags:
	$(CTAGS) -f $(TAGS) -R

libhblk_blockchain.a: $(OBJ)
	$(AR) $@ $^
