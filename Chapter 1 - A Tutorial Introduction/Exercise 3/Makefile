NAME=tc

output: tempconvert.o
	gcc tempconvert.o -o $(NAME)

tempconvert.o: tempconvert.c
	gcc -c tempconvert.c

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
	