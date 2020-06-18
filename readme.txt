This folder contains the input file, the initial temperature field, and the author's own version of the CitcomS code which are needed to reproduce the geodynamic modeling results.

The files are:
1. citcoms.input: this is input file
2. initial_temperature.tar.gz: the initial temperature field. After unzipping, you get 192 files, with each of them the temperature field for one processor. The initial temperature field is converted from seismic tomography model SEMUCB-WM1. More details are listed in the method section of the paper.
3. CitcomS.tar.gz: the author's own modified version of the CitcomS code. The original code is available online at https://geodynamics.org/cig/software/citcoms/

After compile the code, you get an executable file named CitcomSFull under the CitcomS/bin folder

To run the code, use "mpirun -np 192 CitcomSFull citcoms.input". A new folder namded "UHVZ" is generated, which contain the output data.

Questions about geodynamic models can be sent to Mingming.Li@asu.edu
