all: clean vecAdd_cl

.PHONY: clean

LDLIBS=  -L. \
	 -lm \
    	 -lOpenCL \
    	 -lrt \
    	 -lpthread \
	 -ldl \
	 -lstdc++

vecAdd_cl: vecAdd.c
	mkdir -p bin
	gcc -g -o bin/vecAdd_cl vecAdd.c $(LDLIBS) 

clean:
	rm -rf bin
