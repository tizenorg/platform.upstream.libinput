noinst_PROGRAMS = event-debug

AM_CPPFLAGS = -I$(top_srcdir)/include \
              -I$(top_srcdir)/src

event_debug_SOURCES = event-debug.c
event_debug_LDADD = ../src/libinput.la $(LIBUDEV_LIBS)
event_debug_LDFLAGS = -no-install
event_debug_CFLAGS = $(LIBUDEV_CFLAGS)

if BUILD_EVENTGUI
noinst_PROGRAMS += event-gui

event_gui_SOURCES = event-gui.c
event_gui_LDADD = ../src/libinput.la $(CAIRO_LIBS) $(GTK_LIBS) $(LIBUDEV_LIBS)
event_gui_CFLAGS = $(CAIRO_CFLAGS) $(GTK_CFLAGS) $(LIBUDEV_CFLAGS)
event_gui_LDFLAGS = -no-install
endif
