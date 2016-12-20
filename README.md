Example programm HELLO WORLD!

program hello
	print *, "Hello World!"
end program hello


Compile:

gfortran -c hello.f95


wikibooks.org: https://en.wikibooks.org/wiki/Fortran/Hello_world

#Hello_World.f

Below is a simple Fortran program. You can paste this into a text editor (such as Emacs or Vim.) Source code must be in a plain text file, so don't use a word processor (such as Microsoft Word), because its native format is usually not plain text, or otherwise contains special formatting data.

Give the file a name such as hello.f - common Fortran file suffixes are .f, .FOR, .for, .f77, .f90 and .f95. You may also use .F, .fpp and .FPP (which support Preprocessing).

       program hello
          print *, "Hello World!"
       end program hello

or the archaic but shorter form:

       PRINT *, "Hello World!"
       END

Fixed format source code needs 6 spaces before code begins, but the free source form of Fortran 90 does not.

Because Fortran is case insensitive, one could just as easily write the first 'hello' program as:

      Program Hello
      Print *, "Hello World!"
      End Program Hello

The only case sensitive part of this program is what contained in the quotation marks of the print statement. ("Hello World!")


#Compiling
Unix

There are several Fortran compilers available for Unix. Among the most popular are:

    Fortran 95 optimizing compiler from Oracle Solaris Studio. Invocation:

f95 -o hello hello.f

    G95, a compiler compliant with the Fortran 95 standard. Some of Fortran 2003 standard features are also supported. Invocation:

g95 -o hello hello.f90

    GNU Fortran compiler from the GCC, which is a fork of G95. Invocation:

gfortran -o hello hello.f90

Note: the GNU Fortran compiler uses the Fortran 77 standard by default, so the input file must have the .f90 (or of later standard) suffix, so that the compiler can guess the desired standard automatically. Alternatively you can supply the -ffree-form option with the usual .f suffix to enable free-form format instead of the fixed-form format used by the Fortran 77 standard.

Once the program is compiled and linked, you may execute it:

./hello



