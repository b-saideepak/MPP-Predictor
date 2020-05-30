# Light-weight-ML-DL-Branch-Predictor
Download the CBP-2016 Simulation Infrastructure: http://hpca23.cse.tamu.edu/cbp2016/cbp2016.final.tar.gz <br>
Unpack the kit: <br>
$ tar -xzvf cbp2016.tar.gz <br>
$ cd cbp2016 <br>
There should be five directories: sim, scripts, traces, bin, and results. <br>
You will need to install the BOOST library and add a link to the library to the Makefile in the sim directory. See comments in the Makefile. <br>
You will need to download the evaluation traces: http://hpca23.cse.tamu.edu/cbp2016/evaluationTraces.Final.tar <br>
Extract the traces to cbp2016/traces/ folder <br>
You will have to modify the predictor.h file in sim directory to make changes to the predictor. <br>
Place the predictor.h file in the sim directory. <br>
The sim directory contains the simulator: <br>
$ cd sim <br>
$ make clean; make <br>
The scripts directory contains scripts that can help you run your predictor for all the traces.  Check out the doit.sh file in the scripts directory. <br>
$ cd ../scripts <br>
$ ./doit.sh <br>
The outputs (MPkI) for various traces will be displayed on the screen along with mean MPkI as well as they are generated in detail in results folder. <br>
We have uploaded the original 8.25kB predictor.h file as well as our 2.25kB predictor.h file. You can use them to run the predictor with the above mentioned commands and obtain the results. <br>
