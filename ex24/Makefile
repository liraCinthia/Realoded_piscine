
FILES = $(addprefix srcs/,  ft_putchar.c ft_putstr.c ft_strcmp.c ft_strlen.c ft_swap.c)

#FILES_O = ft_putchar.o ft_putstr.o ft_strcmp.o ft_strlen.o ft_swap.o

FILES_O = $(FILES:%.c=%.o)

all: libft.a


fclean: clean
	rm -f libft.a

clean:
	rm -f $(FILES_O)

re: fclean libft.a


libft.a: $(FILES_O)
	gcc main.c $(FILES_O) -o $@
#       gcc -c $(addprefix srcs/, $(FILES))	


%.o: %.c
	gcc -c $< -o $@ -I includes




#	ranlib $@ - usada para criar um indice na biblioteca
