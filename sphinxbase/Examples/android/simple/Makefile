# DO NOT EDIT: instead edit ../../..//mnt/c/swigwin-3.0.12/Examples/android/simple/Makefile
# and run (cd ../../../ && ./config.status) to regenerate
TOP_BUILDDIR_TO_TOP_SRCDIR = /mnt/c/swigwin-3.0.12/
SRCDIR = ../../..//mnt/c/swigwin-3.0.12/Examples/android/simple/

TOP        = ../..
SWIGEXE    = $(TOP)/../swig
SWIG_LIB_DIR = $(TOP)/../$(TOP_BUILDDIR_TO_TOP_SRCDIR)Lib
TARGET     = example
INTERFACE  = example.i
INTERFACEDIR = jni/
PACKAGEDIR = $(SRCDIR)src/org/swig
PACKAGENAME= org.swig.simple
SWIGOPT    = -package $(PACKAGENAME) -outdir $(PACKAGEDIR)/simple
PROJECTNAME= SwigSimple
TARGETID  = 1
#INSTALLOPTIONS = -s # To install on SD Card

check: build

build:
	$(MAKE) -f $(TOP)/Makefile SRCDIR='$(SRCDIR)' CXXSRCS='$(CXXSRCS)' \
	SWIG_LIB_DIR='$(SWIG_LIB_DIR)' SWIGEXE='$(SWIGEXE)' \
	SWIGOPT='$(SWIGOPT)' TARGET='$(TARGET)' INTERFACE='$(INTERFACE)' INTERFACEDIR='$(INTERFACEDIR)' \
	PROJECTNAME='$(PROJECTNAME)' TARGETID='$(TARGETID)' android

install:
	$(MAKE) -f $(TOP)/Makefile SRCDIR='$(SRCDIR)' INSTALLOPTIONS='$(INSTALLOPTIONS)' PROJECTNAME='$(PROJECTNAME)' \
	PACKAGEDIR='$(PACKAGEDIR)' PACKAGENAME='$(PACKAGENAME)' android_install

clean:
	$(MAKE) -f $(TOP)/Makefile SRCDIR='$(SRCDIR)' TARGET='$(TARGET)' PROJECTNAME='$(PROJECTNAME)' \
	PACKAGEDIR='$(PACKAGEDIR)' INTERFACEDIR='$(INTERFACEDIR)' android_clean
