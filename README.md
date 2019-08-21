csgl
===

#### now you can get more effective generated code tool by project [miniGameEngine](https://github.com/coderguang/miniGameEngine)


* a tools for **generated code** by **flex** and **bison**
* it only run in linux. centos7.0  bison (GNU Bison) 2.7   flex 2.5.37
* it can identify **enum**,**struct**,**interface** and generated serialize for [csglib](https://github.com/coderguang/csglib)

#### how to start
 1. complie it,it use clang for complie
 ```shell
    make
 ```
 2. if make error,check if bison or flex install or not.
 3. start generated code  
    format is ./csgl inputfileDir outputfileDir inputfileName
```shell
  test -d generateCode||mkdir generateCode
  ./csgl ./ generateCode/ Test
```
 4. and then,your can find the generated code in generateCode dir.  
    if success,you will get below output.
```shell
  [root@VM_38_103_centos csgl]# ./csgl ./ generateCode/ Test            
  input file is ./Test.csgl
  output dir is generateCode/
  output headfile is generateCode/Test.h
  output cppfile is generateCode/Test.cpp
  start generated head file Test.csgl
  start generated cpp file Test.csgl
  build csgl file success!
```
  and generator code in generateCode.this code is use for [csglib](https://github.com/coderguang/csglib)



