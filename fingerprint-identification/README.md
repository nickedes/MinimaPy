Fingerprint Identification
==========================
A python script which checks two fingerprint images by using **[OCR](http://en.wikipedia.org/wiki/Optical_character_recognition)**.

## Requirements-
1. Python 3
2. [OpenCV 3.0](http://opencv.org/opencv-3-0-alpha.html)

## Installation
## Opencv 3.0

### Getting the Cutting-edge OpenCV from the Git Repository

Download the git repository [OpenCV repository](https://github.com/Itseez/opencv/tree/3.0.0-alpha).Then extract the repository into your current working directory.

### Build OpenCV from source

Create a temporary directory, which we denote as ```<cmake_binary_dir>```, where you want to put the generated Makefiles, project files as well the object files and output binaries.Then enter the directory and build the code.

For example

```
cd ~/opencv-3.0.0-alpha
mkdir release
cd release
cmake -D CMAKE_BUILD_TYPE=RELEASE -D CMAKE_INSTALL_PREFIX=/usr/local ..
```

Enter the created temporary directory ```(<cmake_binary_dir>)``` and proceed with:

```
make -j8 # -j8 runs 8 jobs in parallel.
         # Change 8 to number of hardware threads available.
sudo make install
```