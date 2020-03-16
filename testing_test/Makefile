#Makefile for Assignment 3 unit tests
#Aander Zimmermann ZMMALE001

CC=g++
CCFLAGS=-std=c++11

SRC = ../src/unitTests/UnitTesting.cpp \
        ../src/unitTests/catch.hpp \
		../src/huffmanCode/huffmanTree.cpp \
        ../src/huffmanCode/huffmanTree.h \
        ../src/huffmanCode/huffmanNode.cpp \
        ../src/huffmanCode/huffmanNode.h \
        ../src/huffmanCode/huffmanEncode.cpp \
        ../src/huffmanCode/huffmanEncode.h \
        ../src/huffmanCode/huffmanDecode.cpp \
        ../src/huffmanCode/huffmanDecode.h \
        ../src/bitstream/BitIn.cpp \
        ../src/bitstream/BitIn.h \
        ../src/bitstream/BitOut.cpp \
        ../src/bitstream/BitOut.h \

OBJ = $(SRC:.cpp=.o)

PROG = unitTesting

$(PROG) : $(OBJ)
	$(CC) $(CCFLAGS) $(SRC) -o unitTesting
	
.cpp.o:
	$(CC) $(CCFLAGS) -c $<

depend:
	$(CC) -M $(SRC) > incl.defs

# clean
clean:
	rm -f *.o
	rm -f unitTesting