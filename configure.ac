AC_INIT([QuantumXML], [0.1], [sigsegv@quantumfish.com], [QuantumXML], [http://www.quantumfish.com/])
AC_PREREQ([2.59])
AM_INIT_AUTOMAKE([1.10 -Wall no-define])
AC_PROG_CXX
AC_PROG_LIBTOOL
LT_INIT([disable-static])

AC_HEADER_STDC
AC_CHECK_HEADERS([string])
AC_CHECK_HEADERS([iostream])

# use pkg-config
PKG_PROG_PKG_CONFIG([0.2])

# checks for libraries which use pkg-config

# libv3dimage needs libpng support
PKG_CHECK_MODULES([libpng], [libpng])

# need log4cxx for logging support
PKG_CHECK_MODULES([liblog4cxx], [liblog4cxx])

# libv3dfont needs freetype2
PKG_CHECK_MODULES([freetype2], [freetype2])

# libv3daudio needs openal
PKG_CHECK_MODULES([openal], [openal])
PKG_CHECK_MODULES([freealut], [freealut])

# libhookah needs sdl
PKG_CHECK_MODULES([sdl], [sdl])

# gcov support (for code coverage reports)

AC_PATH_PROG([GCOV], [gcov], [enable_gcov=no])

AC_MSG_CHECKING([whether to build with gcov testing])

AC_ARG_ENABLE([gcov],
              [AS_HELP_STRING([--enable-gcov],
                              [Whether to enable coverage testing (requires gcc and gcov)])],
              [],
              [enable_gcov=no])

AS_IF([test "x$enable_gcov" = "xyes" && test "x$GCC" = "xyes"],
      [
        GCOV_CFLAGS="-g -O0 -fprofile-arcs -ftest-coverage"
        GCOV_LDFLAGS="-lgcov"
      ]
)

AM_CONDITIONAL([GCOV_ENABLED], [test "x$enable_gcov" = "xyes"])
AC_SUBST([GCOV_CFLAGS])
AC_SUBST([GCOV_LDFLAGS])
AC_MSG_RESULT([$enable_gcov])


AC_SUBST([QUANTUMXML_SO_VERSION], [0:1:0])
AC_SUBST([QUANTUMXML_API_VERSION], [1.0])

# save configure options in config.nice
QUANTUMXML_CONFIG_NICE([config.nice])

AC_CONFIG_FILES([
Makefile 
QuantumXML-1.0.pc
])

AC_OUTPUT

