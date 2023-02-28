# The-source-code-for-searching-RKD-Trails-of-SIMON-and-SIMECK
There are 4 files in this repository：  
* Simeck32_64_Valid_RKD_Cryptanalysis.cpp
* Simeck48_96_Valid_RKD_Cryptanalysis.cpp
* Simeck64_128_Valid_RKD_Cryptanalysis.cpp  
* Simon128_256_Valid_RKD_Cryptanalysis.cpp
# Instructions for Execution 
For example, to search for a valid RKD trails with a Hamming weight of 30 in 14 rounds for simeck32, you can execute the program according to the following command to obtain：

```C++ simeck32-valid-RKD-trail.cpp -o a```  
```./a 14 30 >14-30.smt2```  
```time bitwuzla --hex 14-30.smt2 >14-30.txt```
  
   
*Simeck48_96_Valid_RKD_Cryptanalysis.cpp*, *Simeck64_128_Valid_RKD_Cryptanalysis.cpp* and *Simon128_256_Valid_RKD_Cryptanalysis.cpp* operate like *Simeck32_64_Valid_RKD_Cryptanalysis.cpp*
