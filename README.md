### Use another_build_copy/orocos_kinematics_dynamics

## Install Sip
```bash  

cd sip-4.19.3
python configure.py
make -j8; sudo make install
```
```bash (python 3)
pip install PyQt5-sip;
pip install sip
```
```bash (KDL C++) 
export ROS_PYTHON_VERSION=3
cd ../orocos_kdl
mkdir build; cd build;
cmake ..
make -j8; sudo make install
```
```bash (Python Binding C++) 
add the anaconda python path to ../../python_orocos_kdl/CMakeList.txt
```bash
 
```
```
cd ../../python_orocos_kdl
mkdir build; cd build;
cmake ..  -DPYTHON_VERSION=3.6.9 -DPYTHON_EXECUTABLE=~/anaconda2/envs/omg/bin/python3.6
make -j8;  cp PyKDL.so ~/anaconda2/envs/omg/lib/python3.6/site-packages/
```


