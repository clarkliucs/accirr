include ../Makefile

PCM_DEPEND += cpucounters.cpp client_bw.cpp pci.cpp msr.cpp utils.cpp

PREFETCH := -DDATA_PREFETCH

MODE := -DPREFECH_MODE=1

LOCALICY := -DPREFETCH_LOCALITY=3

CXXFLAGS += $(PREFETCH) $(MODE) $(LOCALICY) -pthread -lrt -DUSING_MALLOC
TARGET=hello_world

all:$(TARGET)

hello_world:$(DEPEND) $(LIB)


.PHONY:clean
clean:
	rm -rf $(TARGET)

