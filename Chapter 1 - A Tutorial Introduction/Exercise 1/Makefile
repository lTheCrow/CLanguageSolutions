NAME=hw

output: helloworld.o
	gcc helloworld.o -o $(NAME)

helloworld.o: helloworld.c
	gcc -c helloworld.c

clean:
ifeq ($(OS),Windows_NT)
	del *.o
else
	rm *.o
endif

run:
ifeq ($(OS),Windows_NT)
	$(NAME).exe
else
	./$(NAME)
endif
