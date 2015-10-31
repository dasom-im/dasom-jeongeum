moduledir = `pkg-config --variable=libdir dasom`/dasom/modules
module_LTLIBRARIES = dasom-jeongeum.la

gsettings_SCHEMAS = org.freedesktop.Dasom.engines.jeongeum.gschema.xml
@GSETTINGS_RULES@

dasom_jeongeum_la_SOURCES = dasom-jeongeum.c dasom-jeongeum.h
dasom_jeongeum_la_CFLAGS  = \
	-Wall -Werror \
	-DG_LOG_DOMAIN=\"dasom\" \
	$(DASOM_JEONGEUM_DEPS_CFLAGS)

dasom_jeongeum_la_LDFLAGS = -avoid-version -module $(DASOM_JEONGEUM_DEPS_LIBS)

DISTCLEANFILES = Makefile.in

install-data-hook:
	chmod -x $(DESTDIR)$(moduledir)/dasom-jeongeum.so
	rm    -f $(DESTDIR)$(moduledir)/dasom-jeongeum.la

uninstall-hook:
	-rm -f $(DESTDIR)$(moduledir)/dasom-jeongeum.so
	-rmdir $(DESTDIR)$(moduledir)
