AC_INIT([Helloworld C++], [0.5], [bug-report@hello.example.com],
             [helloworld_cc], [http://hello.example.com/])
AC_PREREQ([2.59])
AM_INIT_AUTOMAKE([1.10 -Wall no-define foreign])
AC_CONFIG_HEADERS([config.h])
AC_PROG_CXX
AC_CHECK_LIB([m],[cos])
AC_CHECK_LIB([gslcblas],[cblas_dgemm])
AC_CHECK_LIB([gsl],[gsl_blas_dgemm])
AC_CONFIG_FILES([Makefile])
AC_OUTPUT
