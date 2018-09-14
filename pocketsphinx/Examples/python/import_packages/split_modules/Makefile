# DO NOT EDIT: instead edit ../../../..//mnt/c/swigwin-3.0.12/Examples/python/import_packages/split_modules/Makefile
# and run (cd ../../../../ && ./config.status) to regenerate
TOP_BUILDDIR_TO_TOP_SRCDIR = /mnt/c/swigwin-3.0.12/
SRCDIR = ../../../..//mnt/c/swigwin-3.0.12/Examples/python/import_packages/split_modules/

TOP        = ../../..
LIBS       =

subdirs = vanilla vanilla_split


check: build
	for s in $(subdirs); do \
		(cd $$s && $(MAKE) check); \
	done

build:
	for s in $(subdirs); do \
		(cd $$s && $(MAKE) SWIGOPT='$(SWIGOPT)' LIBS='$(LIBS)' build); \
	done

static:
	for s in $(subdirs); do \
		(cd $$s && $(MAKE) SWIGOPT='$(SWIGOPT)' LIBS='$(LIBS)' static); \
	done

clean:
	$(MAKE) -f $(TOP)/Makefile SRCDIR='$(SRCDIR)' python_clean
	for s in $(subdirs); do \
		(cd $$s && $(MAKE) clean); \
	done
