# Post Release Notes for PSOPT Release 2 #


## PSOPT Release 2 Patch 02 ##

### Description ###

This patch fixes problems with the 'rk4\_propagate' and 'rkf\_propagate' functions.

This patch may be downloaded from:

http://psopt.googlecode.com/files/patch_2.02.zip

Date of Release of this patch: 31 July 2010

### Applying the patch ###

This is a simple procedure.

1) Extract the contents of the archive patch\_2.02.zip. This will create

> a directory ./patch\_2.02

2) Copy the the files "./patch\_2.02/psopt.cxx" and "./patch\_2.02/psopt.h"  into the directory   

&lt;BASEDIR&gt;

/psopt2/PSOPT/src, replacing the original files "psopt.**" located in that directory, where**

&lt;BASEDIR&gt;

 is the directory where the original source distribution of PSOPT was extracted.

3) Depending on your operating system, do

> a) From Ubuntu Linux:

> - Open a terminal and cd to the directory 

&lt;BASEDIR&gt;

/psopt2/PSOPT/lib

> - Enter the command

> $ make

> b) From Microsoft Windows:

> - Open a MS Visual Studio command prompt and cd to the directory

> 

&lt;BASEDIR&gt;

\psopt2\PSOPT\lib

> - Enter the command

> > nmake -f Makefile.vc all



## PSOPT Release 2 Patch 01 ##

### Description ###

This patch fixes a problem which may arise with optimal control problems with a non-zero cost integrand. It may happen that the integral of the cost is not evaluated in problems when it should be evaluated. The problem does not show with the examples provided with PSOPT release 2, but may occur in other problems.

This patch may be downloaded from:

http://psopt.googlecode.com/files/patch_2.01.tgz

Date of Release of this patch: 08 March 2010

### Applying the patch ###

This is a simple procedure.

1) Extract the contents of the archive patch\_2.01.tgz. This will create

> a directory ./patch\_2.01

2) Copy the the file "./patch\_2.01/psopt.cxx" into the directory

> 

&lt;BASEDIR&gt;

/psopt2/PSOPT/src, replacing the original file "psopt.cxx" located in that directory, where 

&lt;BASEDIR&gt;

 is the directory where the original source distribution of PSOPT was extracted.

3) Depending on your operating system, do

> a) From Ubuntu Linux:

> - Open a terminal and cd to the directory 

&lt;BASEDIR&gt;

/psopt2/PSOPT/lib

> - Enter the command

> $ make

> b) From Microsoft Windows:

> - Open a MS Visual Studio command prompt and cd to the directory

> 

&lt;BASEDIR&gt;

\psopt2\PSOPT\lib

> - Enter the command

> > nmake -f Makefile.vc all