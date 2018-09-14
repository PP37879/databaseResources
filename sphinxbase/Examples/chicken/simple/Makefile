# DO NOT EDIT: instead edit ../../..//mnt/c/swigwin-3.0.12/Examples/chicken/simple/Makefile
# and run (cd ../../../ && ./config.status) to regenerate
TOP_BUILDDIR_TO_TOP_SRCDIR = /mnt/c/swigwin-3.0.12/
SRCDIR = ../../..//mnt/c/swigwin-3.0.12/Examples/chicken/simple/

TOP        = ../..
SWIGEXE    = $(TOP)/../swig
SWIG_LIB_DIR = $(TOP)/../$(TOP_BUILDDIR_TO_TOP_SRCDIR)Lib
INTERFACE  = example.i
SRCS       = example.c
CXXSRCS    =
TARGET     = simple
INCLUDE    =
SWIGOPT    =
VARIANT    =

# uncomment the following two lines to build a static exe
#CHICKEN_MAIN = runme.scm
#VARIANT    = _static

check: build
	$(MAKE) -f $(TOP)/Makefile SRCDIR='$(SRCDIR)' chicken_run

build: $(TARGET)

$(TARGET): $(INTERFACE) $(SRCS)
	$(MAKE) -f $(TOP)/Makefile SRCDIR='$(SRCDIR)' \
	SRCS='$(SRCS)' CXXSRCS='$(CXXSRCS)' CHICKEN_MAIN='$(CHICKEN_MAIN)' \
	SWIG_LIB_DIR='$(SWIG_LIB_DIR)' SWIGEXE='$(SWIGEXE)' \
	INCLUDE='$(INCLUDE)' SWIGOPT='$(SWIGOPT)' TARGET='$(TARGET)' \
	INTERFACE='$(INTERFACE)' CHICKENOPTS='$(CHICKENOPTS)' chicken$(VARIANT)

clean:
	$(MAKE) -f $(TOP)/Makefile SRCDIR='$(SRCDIR)' chicken_clean
	rm -f example.scm example-generic.scm example-clos.scm
	rm -f $(TARGET)
