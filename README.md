## Install Sip
```bash (python 2)
cd sip-4.19.3
python configure.py
make -j8; sudo make install
```
```bash (python 3)
pip install PyQt5-sip;
pip install sip
```
```bash (KDL C++) 
cd ../orocos_kdl
mkdir build; cd build;
cmake ..
make -j8; sudo make install
```
```bash (Python Binding C++) 
add the anaconda python path to ../../python_orocos_kdl/CMakeList.txt
```bash
SET(PYTHON_VERSION 3.6.9 CACHE STRING "Python Version")
set(PYTHON_EXECUTABLE "/anaconda2/envs/omg/bin/python")
```
```
cd ../../python_orocos_kdl
mkdir build; cd build;
cmake ..  
make -j8; sudo make install
```


