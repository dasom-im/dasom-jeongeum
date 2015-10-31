SUBDIRS = src

ACLOCAL_AMFLAGS = -I m4

DISTCLEANFILES = \
	Makefile.in \
	INSTALL \
	aclocal.m4 \
	config.h.in \
	config.h.in~ \
	configure

clean-local:
	-debian/rules clean

distclean-local:
	rm -rf autom4te.cache build-aux m4

ChangeLog:

.PHONY: ChangeLog
