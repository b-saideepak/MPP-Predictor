# Light-weight-ML-DL-Branch-Predictor
Download the CBP-2016 Simulation Infrastructure from [here](http://hpca23.cse.tamu.edu/cbp2016/cbp2016.final.tar.gz) 

Unpack the kit: 

```bash
$ tar -xzvf cbp2016.tar.gz 
$ cd cbp2016 
```
There should be five directories: sim, scripts, traces, bin, and results. 

You will need to install the BOOST library and add a link to the library to the Makefile in the sim directory. See comments in the Makefile.

You will need to download the evaluation traces from [here](http://hpca23.cse.tamu.edu/cbp2016/evaluationTraces.Final.tar) 

Extract the traces to `cbp2016/traces/` folder 

You will have to place our uploaded `predictor.h` file in `sim` directory. 

We have made all the changes to `predictor.h` file only. 
The `sim` directory contains the simulator: 
```bash
$ cd sim 
$ make clean; make 
```
The `scripts` directory contains scripts that can help you run your predictor for all the traces.  Check out the `doit.sh` file in the scripts directory. 
```bash
$ cd ../scripts 
$ ./doit.sh
```
The outputs (MPkI) for various traces will be displayed on the screen along with mean MPkI as well as they are generated in detail in results folder. 

We have uploaded our 2.25kB `predictor.h` file. You can use it to run the predictor with the above mentioned commands and obtain the results. 

Normally, it will take around 15-20 mins to obtain the results.

You can as well get the original `predictor.h` file from the downloaded infrastructure. 

The location is `/submissions/DanielJimenez1/cbp8KB/predictor.h` 
