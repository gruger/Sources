ACLOCAL_AMFLAGS = -I ../m4

libfindexec_LTLIBRARIES = libfindexec.la libfindexec_g.la
libfindexecdir = $(libdir)/singular

CXXTEMPLFLAGS =  --no-exceptions ## -fno-implicit-templates

libfindexec_la_CFLAGS   = -O3 -fomit-frame-pointer ${PIPE}
libfindexec_g_la_CFLAGS = ${PIPE}

libfindexec_la_CXXFLAGS   = -O3 -fomit-frame-pointer --no-rtti ${PIPE} ${CXXTEMPLFLAGS}
libfindexec_g_la_CXXFLAGS = -g -Wextra -Wall -pedantic -Wno-long-long ${PIPE} ${CXXTEMPLFLAGS}
# -fdiagnostics-show-option 

AM_CPPFLAGS = -I${top_srcdir} -I${top_builddir} 

libfindexec_la_CPPFLAGS   = ${AM_CPPFLAGS} -DHAVE_CONFIG_H -DNDEBUG -DOM_NDEBUG
libfindexec_g_la_CPPFLAGS = ${AM_CPPFLAGS} -DHAVE_CONFIG_H 

SOURCES  = omFindExec.c feResource.cc feFopen.cc
libfindexec_la_SOURCES   = $(SOURCES)
libfindexec_g_la_SOURCES = $(SOURCES)

libfindexec_includedir  =$(includedir)/singular/findexec/

libfindexec_include_HEADERS = omFindExec.h feResource.h feFopen.h



