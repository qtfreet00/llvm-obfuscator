#### Low Level Virtual Machine (LLVM)
================================

This directory and its subdirectories contain source code for LLVM,
a toolkit for the construction of highly optimized compilers,
optimizers, and runtime environments.

LLVM is open source software. You may freely distribute it under the terms of
the license agreement found in LICENSE.txt.

Please see the documentation provided in docs/ for further
assistance with LLVM, and in particular docs/GettingStarted.rst for getting
started with LLVM and docs/README.txt for an overview of LLVM's
documentation setup.

If you are writing a package for LLVM, see docs/Packaging.rst for our
suggestions.

##### Wiki: 

https://github.com/obfuscator-llvm/obfuscator/wiki

##### Build:

  * git clone https://github.com/Qrilee/llvm-obfuscator
  
  * mkdir build
  
  * cd build
  
  * cmake -DCMAKE_BUILD_TYPE=Release ../Obfuscator-LLVM/
  
  * make -j7
  
  Build pass for windows:
  
     MinGW64 for Windows
     
     Cmake 3.9 rc5 for Windows x64
     
  Build pass for linux:
  
     gcc&g++ 7.2.0
     
     cmake 3.8.0
     
##### Use:

-mllvm -bcf -mllvm -fla -mllvm -sub -mllvm -sobf
  
##### Function:

* Instructions Substitution -mllvm -sub
* Bogus Control Flow -mllvm -bcf
* Control Flow Flattening -mllvm -fla
* String Obfuscation -mllvm -sobf
