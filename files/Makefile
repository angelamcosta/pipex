NAME	=	pipex

CC		=	cc
CFLAGS	=	-Wall -Werror -Wextra
RM		=	rm -f

SRC		=	pipex.c

OBJ		=	$(SRC:.c=.o)

all:		$(NAME)

$(NAME):	$(OBJ)
			ar -r $(NAME) $(OBJ)

clean:
			$(RM) $(OBJ)

fclean:		clean
			$(RM) $(NAME)

re:			fclean all