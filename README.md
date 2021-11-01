# tensorflow-2.X-for-Xilinx-Pynq-Z2
This tutorial focuses to successfully install tensorflow 2.X versions for Xilinx Pynq

First load boot image for the Pynq. The boot image can be found here (http://www.pynq.io/board.html) 
* Here the boot image of v2.6 for the Pynq z2 has been loaded.
* # get a fresh start
  $ sudo apt-get update
  $ sudo apt-get upgrade
# remove old versions, if not placed in a virtual environment (let pip search for them)
  $ sudo pip uninstall tensorflow
  $ sudo pip3 uninstall tensorflow
# install the dependencies (if not already onboard)
  $ sudo apt-get install gfortran
  $ sudo apt-get install libhdf5-dev libc-ares-dev libeigen3-dev
  $ sudo apt-get install libatlas-base-dev libopenblas-dev libblas-dev
  $ sudo apt-get install openmpi-bin libopenmpi-dev
  $ sudo apt-get install liblapack-dev cython
  $ sudo pip3 install keras_applications==1.0.8 --no-deps
  $ sudo pip3 install keras_preprocessing==1.1.0 --no-deps
  $ sudo pip3 install -U --user six wheel mock
  $ sudo -H pip3 install pybind11
  $ sudo -H pip3 install h5py==2.10.0
# upgrade setuptools 40.8.0 -> 52.0.0
  $ sudo -H pip3 install --upgrade setuptools
  $ wget 
check you python3 version
  $ python --version
Modify the CP according to the python version. Example if python 3.6.5 is available change cp to cp36
install tensorflow
  $ sudo -H pip3 install tensorflow-2.1.0-cp36-none-linux_armv7l.whl

Check tensorflow
  $ python
> import tensorflow
> print(tensorflow.__version__)
If the versions number shows then tensorflow has been installed and is working.
