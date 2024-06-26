##
## EPITECH PROJECT, 2023
## C-POOL
## File description:
## Makefile.c
##

## ---- LIB ----

HANDLER_FOLDER = handler/
PARSER_FOLDER = parser/
CONVERSION_FOLDER = $(HANDLER_FOLDER)conversion/
PRECISION_FOLDER = $(HANDLER_FOLDER)precision/
WIDTH_FOLDER = $(HANDLER_FOLDER)/width/
FLAG_FOLDER = $(HANDLER_FOLDER)/flags/

LIB_FOLDER = ./lib/my
LIB_NAME = libmy
LIB = $(LIB_NAME).a

LIB_SRC  = $(LIB_FOLDER)/my_str_isprintable.c
LIB_SRC += $(LIB_FOLDER)/my_showstr.c
LIB_SRC += $(LIB_FOLDER)/my_str_isalpha.c
LIB_SRC += $(LIB_FOLDER)/my_str_islower.c
LIB_SRC += $(LIB_FOLDER)/my_compute_square_root.c
LIB_SRC += $(LIB_FOLDER)/my_strncmp.c
LIB_SRC += $(LIB_FOLDER)/my_strcat.c
LIB_SRC += $(LIB_FOLDER)/my_putchar.c
LIB_SRC += $(LIB_FOLDER)/my_strstr.c
LIB_SRC += $(LIB_FOLDER)/my_str_to_word_array.c
LIB_SRC += $(LIB_FOLDER)/my_compute_power_rec.c
LIB_SRC += $(LIB_FOLDER)/my_put_nbr.c
LIB_SRC += $(LIB_FOLDER)/my_put_double.c
LIB_SRC += $(LIB_FOLDER)/my_getnbr.c
LIB_SRC += $(LIB_FOLDER)/my_swap.c
LIB_SRC += $(LIB_FOLDER)/my_strcmp.c
LIB_SRC += $(LIB_FOLDER)/my_strncat.c
LIB_SRC += $(LIB_FOLDER)/my_strcapitalize.c
LIB_SRC += $(LIB_FOLDER)/my_str_isnum.c
LIB_SRC += $(LIB_FOLDER)/my_strlowcase.c
LIB_SRC += $(LIB_FOLDER)/my_putstr.c
LIB_SRC += $(LIB_FOLDER)/my_libs/my_charlib.c
LIB_SRC += $(LIB_FOLDER)/my_libs/my_islib.c
LIB_SRC += $(LIB_FOLDER)/my_libs/my_mathlib.c
LIB_SRC += $(LIB_FOLDER)/my_libs/my_get_base.c
LIB_SRC += $(LIB_FOLDER)/my_isneg.c
LIB_SRC += $(LIB_FOLDER)/my_show_word_array.c
LIB_SRC += $(LIB_FOLDER)/my_strcpy.c
LIB_SRC += $(LIB_FOLDER)/my_revstr.c
LIB_SRC += $(LIB_FOLDER)/my_is_prime.c
LIB_SRC += $(LIB_FOLDER)/my_showmem.c
LIB_SRC += $(LIB_FOLDER)/my_strncpy.c
LIB_SRC += $(LIB_FOLDER)/my_strlen.c
LIB_SRC += $(LIB_FOLDER)/my_str_isupper.c
LIB_SRC += $(LIB_FOLDER)/my_strupcase.c
LIB_SRC += $(LIB_FOLDER)/my_sort_int_array.c
LIB_SRC += $(LIB_FOLDER)/my_find_prime_sup.c
LIB_SRC += $(LIB_FOLDER)/my_strdup.c
LIB_SRC += $(LIB_FOLDER)/my_strrchr.c
LIB_SRC += my_printf.c
LIB_SRC += get_conv_tab.c
LIB_SRC += linked_list.c
LIB_SRC += my_tab.c
LIB_SRC += $(PARSER_FOLDER)/parser.c
LIB_SRC += $(PARSER_FOLDER)/parser_conversion.c
LIB_SRC += $(PARSER_FOLDER)/parser_flag.c
LIB_SRC += $(PARSER_FOLDER)/parser_length_modifier.c
LIB_SRC += $(PARSER_FOLDER)/parser_precision.c
LIB_SRC += $(PARSER_FOLDER)/parser_width.c
LIB_SRC += $(CONVERSION_FOLDER)/handle_char.c
LIB_SRC += $(CONVERSION_FOLDER)/handle_str.c
LIB_SRC += $(CONVERSION_FOLDER)/handle_int.c
LIB_SRC += $(CONVERSION_FOLDER)/handle_double.c
LIB_SRC += $(CONVERSION_FOLDER)/handle_n.c
LIB_SRC += $(CONVERSION_FOLDER)/handle_binary.c
LIB_SRC += $(CONVERSION_FOLDER)/handle_hexa.c
LIB_SRC += $(CONVERSION_FOLDER)/handle_octal.c
LIB_SRC += $(CONVERSION_FOLDER)/handle_pointer.c
LIB_SRC += $(CONVERSION_FOLDER)/handle_e.c
LIB_SRC += $(CONVERSION_FOLDER)/handle_percent.c
LIB_SRC += $(WIDTH_FOLDER)/handle_width.c
LIB_SRC += $(WIDTH_FOLDER)/handle_width_char.c
LIB_SRC += $(WIDTH_FOLDER)/handle_width_double.c
LIB_SRC += $(WIDTH_FOLDER)/handle_width_str.c
LIB_SRC += $(WIDTH_FOLDER)/handle_width_int.c
LIB_SRC += $(PRECISION_FOLDER)/handle_precision.c
LIB_SRC += $(PRECISION_FOLDER)/handle_precision_d.c
LIB_SRC += $(PRECISION_FOLDER)/handle_precision_s.c
LIB_SRC += $(FLAG_FOLDER)/handle_flag_minus.c
LIB_SRC += $(FLAG_FOLDER)/handle_flag_minus_s.c
LIB_SRC += $(FLAG_FOLDER)/handle_flag_minus_d.c
LIB_SRC += $(FLAG_FOLDER)/handle_flag_minus_c.c
LIB_SRC += $(FLAG_FOLDER)/handle_flag_minus_f.c
LIB_SRC += $(FLAG_FOLDER)/handle_flag_minus_x.c
LIB_SRC += $(FLAG_FOLDER)/handle_flag_minus_o.c

LIB_OBJ	= $(LIB_SRC:.c=.o)

LDFLAGS	= -L. -lmy -lcriterion

TESTS_FLAGS	= -Wall -Wextra --coverage -I include/

TEST_SRC =	tests/test_d_i.c
TEST_SRC +=	tests/test_s.c
TEST_SRC +=	tests/test_f.c
TEST_SRC +=	tests/test_u.c
TEST_SRC +=	tests/test_c.c
TEST_SRC +=	tests/test_x.c

TEST_OBJ =	$(TEST_SRC:.c=.o)

TEST_NAME = unit_test

all: $(LIB)
.PHONY:all

$(LIB): $(LIB_OBJ)
	$(AR) rc $(LIB) $(LIB_OBJ)

tests_run:
	cd tests/
	gcc $(TEST_SRC) -o $(TEST_NAME) $(LDFLAGS) $(TESTS_FLAGS)
	./$(TEST_NAME) --always-succeed

clean:
	$(RM) $(LIB_OBJ)
.PHONY:clean

fclean: clean
	$(RM) -f $(LIB_NAME)
.PHONY:fclean

re: fclean all
.PHONY:re
