objects = addition.o division.o main.o multiplication.o subtraction.o

calculator: $(objects)
	cc -o calculator $(objects)

$(objects): %.o:%.c operations.h
	cc -c $< -o $@

clean:
	rm -rf calculator $(objects)

.PHONY: clean
