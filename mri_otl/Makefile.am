##
## Makefile.am 
##

AM_CFLAGS=-I$(top_srcdir)/include
AM_CXXFLAGS=-I$(top_srcdir)/include

bin_PROGRAMS = list_otl_labels
list_otl_labels_SOURCES= list_otl_labels.c
list_otl_labels_LDADD= $(addprefix $(top_builddir)/, $(LIBS_MGH))
list_otl_labels_LDFLAGS=$(OS_LDFLAGS)

# Our release target. Include files to be excluded here. They will be
# found and removed after 'make install' is run during the 'make
# release' target.
EXCLUDE_FILES="" 
include $(top_srcdir)/Makefile.extra
