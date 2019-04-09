Error installing spatialSEIR package in R on Ubuntu
========================================

Those who are having problems on installing packages in R regarding EBOLA (grantbrown) may get some help from here.


1) For Parallel Package -->>>>>>>>>
==>> In R type 
     require(parallel)      .......as parallel package is part of R Distribution


2) For XML Package -->>>>>>>>>>>
To install curl and xml on ubuntu. 

Run on Terminal
sudo apt-get install libcurl4-openssl-dev   &
sudo apt-get install libxml2-dev

The error messages on package install in R indicate that the curl and xml libraries are not present or cannot be found.


3) For SpatialSEIR Package -->>>>>>>>>
Source:   https://github.com/grantbrown/libspatialSEIR/wiki/installation

The following packages are required:
git
cmake
libboost-dev
libboost-random-dev
r-base-core
r-base-dev
If you have administrator access, these can be installed by running:

sudo apt-get install git cmake libboost-dev libboost-random-dev r-base-core r-base-dev      

Next, you'll need to install the Rcpp R package. From the command line you can start R and install the package in the usual way:

R
>install.packages("Rcpp")  

Then you're ready to clone a copy of the libSpatialSEIR repository and install the associated R package. 
Change to the directory you'd like to create the libSpatialSEIR project folder in and type:

git clone https://github.com/grantbrown/libspatialSEIR.git --recursive
cd libspatialSEIR/R/release_package
./install.sh
 



