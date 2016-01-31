## Updated Microsoft Visual Studio include file ##

Please note that an updated Microsoft Visual Studio include file has been posted in the downloads page. This is for use in Windows installations. The file assumes by default that Microsoft Visual Studio v.10 is being used.

## Detailed instruction for PSOPT installation under Windows ##

Musa Audu from Case Western Reserve University has posted a document with detailed instruction for a successful PSOPT3 installation under Windows. See this link
http://filer.case.edu/mxa93/PSOPT3/


#summary Post release Notes for PSOPT Release 3
# Post Release Notes for PSOPT Release 3 #


## Correction to installation instructions under Ubuntu Linux ##

In page 49 of the PSOPT Release 3 User Manual, the two lines:

$ sudo cp /adolc base/lib64/**/usr/lib**

$ sudo cp -r /adolc base/include/**/usr/include/**

should be:

$ sudo cp ~/adolc base/lib64/**/usr/lib**

$ sudo cp -r ~/adolc base/include/**/usr/include/**

As ADOL-C is installed in the home directory.


## PSOPT Release 3 Patch 01 ##

### Description ###


This patch fixes a problem with the smooth\_sign() function which prevents
the "Coulomb" example to link successfully.

The patch can be downloaded from:

http://psopt.googlecode.com/files/patch_3.01.tgz


Date of Release of this patch: 29 July 2011


### Applying the patch ###



This is a simple procedure.

1) Extract the contents of the archive patch\_2.01.tgz. This will create
> a directory ./patch\_3.01

2) Copy the the file "./patch\_3.01/psopt.cxx"
> into the directory
> 

&lt;BASEDIR&gt;

/Psopt3/PSOPT/src, replacing the original files
> "psopt.cxx" located in that directory, where 

&lt;BASEDIR&gt;

 is the directory
> where the original source distribution of PSOPT was extracted.

3) Depending on your operating system, do
> a) From Ubuntu Linux:
> - Open a terminal and cd to the directory 

&lt;BASEDIR&gt;

/psopt3/PSOPT/lib
> > - Enter the command
> > > $ make


> b) From Microsoft Windows:
> - Open a MS Visual Studio command prompt and cd to the directory
> > 

&lt;BASEDIR&gt;

\Psopt3\PSOPT\lib
> > - Enter the command
> > > > nmake -f Makefile.vc all