NAME=hw

output: helloworld.o
	gcc helloworld.o -o $(NAME)

helloworld.o: helloworld.c
	gcc -c helloworld.c

clean:
ifeq ($(OS),Windows_NT)
	cls
	del *.o
else
	clear
	rm *.o
endif

clean_exe:
ifeq ($(OS),Windows_NT)
	del *.exe
else
	clear
	rm *.exe
endif

run:
ifeq ($(OS),Windows_NT)
	$(NAME).exe
else
	./$(NAME)
endif
