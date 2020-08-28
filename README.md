# Q-Pix RTD signal simulation

Simulatin to get the response of qpix in LAr

This package requires ROOT to be setup, and uses C++17. 
The software versions this was developed with are
cmake version 3.15.5
make  version 3.81
ROOT  Version: 6.18/04


### Building

After you clone the repo the setup.sh script should set up the enviorment and run cmake. Which will compile the project.
You will need to run this setup every time you launch a new terminal. 
```bash
bash setup.sh
```
This will make a build directory and run cmake and make, inorder to make a joint libary that will be moved into the Libary folder. 
Once this is done the example can be tested


### Example
The example will run through 100 marly events that were generated with the geant4 package.
It will run through all functions to produce a QPIX response. It takes an input file fom the geant4 step and outputs a file that is similar to an expected output with a pixel location and reset time. and output a new root file. 

Once the enviorment is sourced the example can be made and ran by.
```bash
cd EXAMPLE
make 
./EXAMPLE
```

![alt text](https://github.com/Q-Pix/Q_PIX_RTD/RTD_Flow.pdf)
