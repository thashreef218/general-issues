# general-issues
**How to copy workspace from one to another**
This tutorial shows how to avoid catkin_make issues while copying catkin workspace to another system.
You can copy packages since it has no relationship between the workspace and I hope it won't throw any error but when you copy workspace  and then you try for a catkin_make then you may get error like this
```
CMake Error: The current CMakeCache.txt directory /home/thashri/AR Projects/real_ws/build/CMakeCache.txt is different than the directory /home/arjun/Agribot2022-main/real_ws/build where CMakeCache.txt was created. This may result in binaries being created in the wrong place. If you are not sure, reedit the CMakeCache.txt
```

So in order to solve this try run below commands
```
ls -l
```
```
rm -rf build/ devel/
```
then
```
catkin_make
```
Hopefully it will work .Good luck

