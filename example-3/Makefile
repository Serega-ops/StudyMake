SOURCE = Kazino-Royal.cpp
RELEASE_EXEC = kazino
DEBUG_EXEC = kazino-dbg

RELEASE_FLAGS = -O2 -Wall
DEBUG_FLAGS = -g -O0 -Wall

.PHONY: all debug release clean

all: release

release: $(RELEASE_EXEC)

$(RELEASE_EXEC): $(SOURCE)
	g++ $(RELEASE_FLAGS) $(SOURCE) -o $(RELEASE_EXEC)

debug: $(DEBUG_EXEC)

$(DEBUG_EXEC): $(SOURCE)
	g++ $(DEBUG_FLAGS) $(SOURCE) -o $(DEBUG_EXEC)

clean:
	rm -f $(RELEASE_EXEC) $(DEBUG_EXEC) *.o
