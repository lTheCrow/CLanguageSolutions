NAME=tc

output: celtofahr.o
	gcc celtofahr.o -o $(NAME)

celtofahr.o: celtofahr.c
	gcc -c celtofahr.c

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
	