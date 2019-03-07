all: clean vecAdd_cu deviceQuery 

.PHONY: clean

vecAdd_cu: vecAdd.cu
	mkdir -p bin
	nvcc -arch=sm_35 -o bin/vecAdd_cu vecAdd.cu

deviceQuery: deviceQuery.cpp
	mkdir -p bin
	nvcc -arch=sm_35 -o bin/deviceQuery -I. deviceQuery.cpp

clean:
	rm -rf bin
