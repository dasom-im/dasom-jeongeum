dnl Process this file with autoconf to produce a configure script.

AC_INIT(dasom-jeongeum, 1.0.1,
        https://github.com/dasom-im/dasom-jeongeum/issues)

AC_CONFIG_HEADERS([config.h])
AC_CONFIG_MACRO_DIR([m4])
AC_CONFIG_AUX_DIR([build-aux])

AM_INIT_AUTOMAKE([-Wall -Werror])
AM_MAINTAINER_MODE([disable])
AM_SILENT_RULES([yes])

AM_PROG_AR
AC_PROG_CC

LT_INIT([disable-static])

PKG_CHECK_MODULES(DASOM_JEONGEUM_DEPS, [libhangul >= 0.0.12 dasom])

GLIB_GSETTINGS

AC_OUTPUT([
  Makefile
  src/Makefile])
