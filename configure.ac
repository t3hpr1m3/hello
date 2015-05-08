AC_PREREQ([2.69])
AC_INIT([codex], [0.0.1], [jdubz@firma8.com])
AC_CONFIG_HEADERS([config.h])

AM_INIT_AUTOMAKE([-Wall])

# Checks for programs.
AC_PROG_CC

AC_MSG_CHECKING([pkg-config m4 macros])
if test m4_ifdef([PKG_CHECK_MODULES], [yes], [no]) == yes; then
	AC_MSG_RESULT([yes])
else
	AC_MSG_RESULT([no])
	AC_MSG_ERROR([pkg-config is required.])
fi

PKG_CHECK_MODULES([HIREDIS], [hiredis >= 0.11])

AC_CONFIG_FILES([Makefile src/Makefile])

AC_OUTPUT
