NAME=pa

output: printargument.o
	gcc printargument.o -o $(NAME)

printargument.o: printargument.c
	gcc -c printargument.c

clean:
ifeq ($(OS),Windows_NT)
	cls
	del *.o
else
	clear
	rm *.o
endif

run:
ifeq ($(OS),Windows_NT)
	$(NAME).exe
else
	./$(NAME)
endif
	