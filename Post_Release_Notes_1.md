# Post release notes for PSOPT Release 1 Build 2009-15-05 #

These notes have been produced after release 1 of PSOPT was published.


**1** There is an issue with the **Linux** Makefiles, which can be solved easily.
The simplest solution to this problem is to create a symbolic link in the home
directory to your home directory. Open a command window and enter the following
command  (which will require the administrator's password):
```
> sudo ln -s /home/USER /home/shs99vmb
```
where USER is the name of your home directory (usually your username).


**2** It seems that the CXSparse makefile was updated on 20 May 2009, which
causes an error when trying to build PSOPT under **Linux**. The solution is simple:

After performing step 11 in page 33 of the PSOPT user manual, please download
the following file:

http://www.cise.ufl.edu/research/sparse/UFconfig/current/UFconfig.tar.gz

Copy the file to the Psopt1 directory and extract it there as follows:
```
> tar zxvf UFconfig.tar.gz
```


**3** Again if you are compiling under **Linux** and do not have SNOPT, please do the following after extracting the Psopt1.tgz archive and having followed notes 1 and 2 above:

  * a) Download the file [use\_ipopt\_only.sh](http://www.reading.ac.uk/~shs99vmb/files/use_ipopt_only.sh) and use it to replace the file **./Psopt1/use\_ipopt\_only.sh** in the
directory where the PSOPT distribution was extracted.

  * b) Download the file [Makefile.ipopt](http://www.reading.ac.uk/~shs99vmb/files/Makefile.ipopt) and use it to replace the file **./Psopt1/PSOPT/examples/Makefile.ipopt**
(note carefully the path).

  * c) Open a command window and cd to the top installation directory (Psopt1). Then run the script:
```
>  sh  ./use_ipopt_only.sh
```

  * d) Now enter the following command from the top installation directory (Psopt1):
```
>  make all
```