CXX=g++
CPPFLAGS=-g -std=c++11 -fopenmp
LIBSEARCHPATH=-L/opt/local/lib/

OBJECTS=$(PROJECT).o Bitmap.o CoordSystem.o ChaoticMap.o LogisticMap.o Histogram.o BifurcationDiagram.o GaussMap.o TentMap.o Zoom.o
PROJECT=main

$(PROJECT) : $(OBJECTS)
	$(CXX) $(CPPFLAGS) $(OBJECTS) -o $@ $(LIBSEARCHPATH) $(LIBS)

.cpp.o :
	$(CXX) -c $(CPPFLAGS) -o $@ $< 

clean :
	rm -f $(OBJECTS)
