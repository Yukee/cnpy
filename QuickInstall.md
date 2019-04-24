To quickly install (using the Intel compiler), move to the instal_dir, and do:
```
source cmake_intel
make cnpy
```

Then in the project you want to use the library in, in CMakeLists.txt add
```
include_directories( instal_dir )
link_directories( instal_dir )
```
and 
```
add_executable(your_exec your_exec.cc)
target_link_libraries(your_exec cnpy z)
```
