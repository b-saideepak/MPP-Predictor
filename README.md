# Light-weight-ML-DL-Branch-Predictor
Download the CBP-2016 Simulation Infrastructure: http://hpca23.cse.tamu.edu/cbp2016/cbp2016.final.tar.gz
Unpack the kit: 
$ tar -xzvf cbp2016.tar.gz
$ cd cbp2016
There should be five directories: sim, scripts, traces, bin, and results.
You will need to install the BOOST library and add a link to the library to the Makefile in the sim directory. See comments in the Makefile. 
You will need to download the evaluation traces: http://hpca23.cse.tamu.edu/cbp2016/evaluationTraces.Final.tar
Extract the traces to cbp2016/traces/ folder
You will have to modify the predictor.h file in sim directory to make changes to the predictor.
Place the predictor.h file in the sim directory.
The sim directory contains the simulator:
$ cd sim
$ make clean; make
The scripts directory contains scripts that can help you run your predictor for all the traces.  Check out the doit.sh file in the scripts directory.
$ cd ../scripts
$ ./doit.sh
The outputs (MPkI) for various traces will be displayed on the screen along with mean MPkI as well as they are generated in detail in results folder.
We have uploaded the original 8.25kB predictor.h file as well as our 2.25kB predictor.h file. You can use them to run the predictor with the above mentioned commands and obtain the results.
