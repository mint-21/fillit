# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: eidaho <marvin@42.fr>                      +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2019/09/24 10:32:58 by eidaho            #+#    #+#              #
#    Updated: 2019/10/30 18:31:53 by vfearles         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

NAME = libft.a

CCFLAGS = -Wall -Wextra -Werror

FILES = ft_memset.c ft_bzero.c ft_memcpy.c ft_memccpy.c ft_memmove.c ft_memchr.c \
ft_memcmp.c ft_strlen.c ft_strdup.c ft_strcpy.c ft_strncpy.c ft_strcat.c \
ft_strncat.c ft_strchr.c ft_strrchr.c ft_strstr.c ft_strnstr.c ft_strcmp.c \
ft_strncmp.c ft_atoi.c ft_isalpha.c ft_isdigit.c ft_isalnum.c ft_isascii.c \
ft_isprint.c ft_toupper.c ft_tolower.c ft_memalloc.c ft_memdel.c ft_strnew.c \
ft_strdel.c ft_strclr.c ft_striter.c ft_striteri.c ft_strmap.c ft_strmapi.c \
ft_strequ.c ft_strnequ.c ft_strsub.c ft_strjoin.c ft_strtrim.c ft_strsplit.c \
ft_itoa.c ft_putchar.c ft_putstr.c ft_putendl.c ft_putnbr.c ft_putchar_fd.c \
ft_putstr_fd.c ft_putendl_fd.c ft_putnbr_fd.c ft_lstnew.c ft_strlcat.c \
ft_lstdelone.c ft_lstdel.c ft_lstadd.c ft_lstiter.c ft_lstmap.c ft_count_if.c \
ft_div_mod.c ft_floor.c ft_foreach.c ft_sqrt.c ft_lstcount.c ft_lstrev.c

OBJECTS = $(FILES:.c=.o)
OBJ_DIR = obj

all: $(NAME)

$(NAME): compile_libft
	@ar rc $(NAME) $(OBJECTS)
	@ranlib $(NAME)
	@mkdir obj
	@mv $(OBJECTS) $(OBJ_DIR)
	@mv $(NAME) ../

compile_libft:
	@echo Compiling libft...
	@gcc $(CCFLAGS) -c $(FILES)

clean:
	@rm -rf $(OBJ_DIR)

fclean: clean
	@rm -rf ../$(NAME)

re: fclean all
