include @GASNET_CONDUIT_INCLUDE_FILE@

CONDUIT_LIBS = @GASNET_CONDUIT_LIBS@ $(CONDUIT_LIBS)

pyexec_LTLIBRARIES = gasnet.la

gasnet_la_SOURCES = \
  gasnet.c gasnet.h \
  pipeline.cpp pipeline.h \
  rmalloc.c rmalloc.h \
  rpc.c rpc.h
gasnet_la_CPPFLAGS = $(PYTHON_CPPFLAGS) $(GASNET_CPPFLAGS)
gasnet_la_LDFLAGS = $(PYTHON_LDFLAGS) -module $(GASNET_LDFLAGS)
gasnet_la_LIBADD = $(GASNET_LIBS)
