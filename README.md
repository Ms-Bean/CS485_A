# CS485_A

If you have not already recursively cloned the submodules after cloning the repository, run this to get emsdk
```bash
git submodule update --init --recursive
``` 
Next, activate emsdk by running the following
```bash
cd emsdk
./emsdk install latest
./emsdk activate latest
source ./emsdk_env.sh
```
Note: You will have to execute `source ./emsdk_env.sh` every time you log into your linux machine


After this, you should have access to `emcc` which will compile C project to web assembly. Try the following
```bash
emcc test.c -o test.html
```
This should generate 3 files. Host all three in an HTTP server and visit the html page to see the results.

