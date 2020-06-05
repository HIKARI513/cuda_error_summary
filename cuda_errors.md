# RuntimeError: cuda runtime error (999) : unknown error at ..\aten\src\THC\THCGeneral.cpp:50
### Solution:
``` shell
sudo rmmod nvidia_uvm
sudo rmmod nvidia
sudo modprobe nvidia
sudo modprobe nvidia_uvm
```
or
``` shell
sudo nvidia-modprobe -u
```
