all: clean vecAdd_cu deviceQuery 

.PHONY: clean

vecAdd_cu: vecAdd.cu
	mkdir -p bin
	nvcc -o bin/vecAdd_cu vecAdd.cu

deviceQuery: deviceQuery.cpp
	mkdir -p bin
	nvcc -o bin/deviceQuery -I. deviceQuery.cpp

clean:
	rm -rf bin
