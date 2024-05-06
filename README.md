# AUV-AIAPAEC
## Status
Models and LQY/LTR control of an overdriven AUV in Python.

This is a simulator of an overdriven AUV, called AIAPAEC, running in Python. In addition, Conda is used to properly install the necessary libraries.

Conda is an open-source package and environment management system that runs on Windows, macOS, and Linux. Conda quickly installs, runs, and updates packages and their dependencies. 

## Requirements
- Ubuntu
```
    Distributor ID:	Ubuntu
    Description:	Ubuntu 22.04.4 LTS
    Release:	22.04
    Codename:	jammy
```
- Install Python

https://www.python.org/downloads/

- Install the Anaconda 

https://www.anaconda.com/download

## Install
To run the main program main.py the following modules must be installed:
```
pip install numpy
```
```
pip install matplotlib
```
```
pip install scipy 
```

The following packages are installed in the following order:

- slycot 0.5.4
```
pip install slycot
```
or 
```
conda install -c conda-forge slycot
```
https://pypi.org/project/slycot/


- control  0.9.4
```
pip install control
```
https://pypi.org/project/control/


The required Python libraries are necessary for the simulation, in any case check if you have the required libraries.

## Download the simulator
Cloning the archives to GitHub
```
git clone https://github.com/DianaHuallpa/AUV-AIAPAEC.git
```

# Structure to folders

    PyAUVsimulator
    ├── lib                                         # File compilated
    ├── lqg_control                                 # File compilated
    ├── lqg_control_image_outputs                   # File save results
    ├── non_linear_model                            # File compilated
    ├── non_linear_model_image_outputs              # File save results
    ├── real_state_space_and_discretized_control    # File save results
    ├── main.py  

## Instrucciones para ejecutar el simulador
The simulator provides the modes of operation of the nonlinear, linearized model and the overdriven AUV control. To demonstrate the simulator operation, three cases will be considered:

1. Thruster distance configuration (dp1, dp2 and dp3).

2. Non Linear Model: for the visualization of the results the input signals are the forces applied by the thrusters in Newton (Tp1, Tp2, Tp).

3. Linearized Model: Once the non-linear model of the AUV is obtained, the system is linearized with certain initial values (X,U).

4. Controller: the controller calculations are developed using the constants generated by the linearized model but only taking the necessary values to control the linear velocities in surge (u), sway (v) and the angular velocity in Yaw (r).

* Suggestions: 


## License


## Credits


## Thanks

Thanks to the Universidad Nacional de San Agustin de Arequipa.

## Running Package

After you have installed the Python libraries and downloaded the AUV simulator package and placed it on your desktop you can launch it using the following commands:
```
cd PythonSimulatorAUV
python main.py
```
to display the generated folders 

```
ls
```

## References
* https://python-control.readthedocs.io/en/0.9.4/index.html
* https://python-control.readthedocs.io/en/0.9.4/classes.html
