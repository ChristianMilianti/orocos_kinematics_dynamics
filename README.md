## Installation 
```bash
pip install PyQt5-sip (python 3)
cd sip-4.19.3
python configure.py
make -j8; sudo make install
cd ../orocos_kdl
mkdir build; cd build;
cmake ..
make -j8; sudo make install
cd ../../python_orocos_kdl
mkdir build; cd build;
cmake ..  
make -j8; sudo make install
```

Before the last build, add 
```bash
SET(PYTHON_VERSION 3.6.9 CACHE STRING "Python Version")
set(PYTHON_EXECUTABLE "/home/liruiw/anaconda2/envs/omg_2/bin/python")
```
to the CMakeList.txt.