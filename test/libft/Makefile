# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: fmorales <fmorales@student.42.fr>          +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2014/02/22 18:04:37 by fmorales          #+#    #+#              #
#    Updated: 2014/02/22 23:54:02 by fmorales         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

# option

CC = gcc
FLAGS = -Wall -Werror -Wextra

# path

HEADER = includes/
SRCDIR = srcs/

# Files

NAME = libft.a

SRC = ft_atoi.c \
	  ft_bzero.c \
	  ft_isalnum.c \
	  ft_isalpha.c \
	  ft_isascii.c \
	  ft_isdigit.c \
	  ft_isprint.c \
	  ft_itoa.c \
	  ft_lstadd.c \
	  ft_lstdelone.c \
	  ft_lstdel.c \
	  ft_lstiter.c \
	  ft_lstnew.c \
	  ft_lstmap.c \
	  ft_memalloc.c \
	  ft_memccpy.c \
	  ft_memchr.c \
	  ft_memcmp.c \
	  ft_memcpy.c \
	  ft_memdel.c \
	  ft_memmove.c \
	  ft_memset.c \
	  ft_putchar.c \
	  ft_putchar_fd.c \
	  ft_putendl.c \
	  ft_putendl_fd.c \
	  ft_putnbr.c \
	  ft_putnbr_fd.c \
	  ft_putstr.c \
	  ft_putstr_fd.c \
	  ft_strcat.c \
	  ft_strcdup.c \
	  ft_strcmp.c \
	  ft_strcpy.c \
	  ft_strdel.c \
	  ft_strdup.c \
	  ft_strequ.c \
	  ft_striter.c \
	  ft_striteri.c \
	  ft_strjoin.c \
	  ft_strlcat.c \
	  ft_strlen.c \
	  ft_strmap.c \
	  ft_strmapi.c \
	  ft_strncat.c \
	  ft_strchr.c \
	  ft_strclr.c \
	  ft_strncmp.c \
	  ft_strncpy.c \
	  ft_strnequ.c \
	  ft_strnew.c \
	  ft_strnstr.c \
	  ft_strrchr.c \
	  ft_strsplit.c \
	  ft_strstr.c \
	  ft_strsub.c \
	  ft_strtrim.c \
	  ft_tolower.c \
	  ft_toupper.c \
	  ft_deltab_str.c \
	  ft_free_line.c \
	  ft_tabcount.c \
	  ft_isspace.c \
	  ft_str_isint.c \
	  ft_str_countword.c \
	  get_next_line.c
O_FILES = $(SRC:.c=.o)

STATE = Updated

.PHONY: all clean fclean re

all: $(NAME)

$(NAME): $(O_FILES)
	@ranlib $(NAME)
	@echo "\033[3;32m$(NAME) Successfully $(STATE)\033[0m"

%.o: $(SRCDIR)%.c
	@$(CC) -o $@ $(FLAGS) -I $(HEADER) -c $<
	@ar -rcs $(NAME) $@

clean:
	@rm -f $(O_FILES)

fclean: clean
	$(eval STATE = Created)
	@rm -f $(NAME)

re: fclean all
