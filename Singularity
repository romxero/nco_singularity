Bootstrap: docker
From: ubuntu:16.04

%labels
Author "Randall Cab White - rcwhite@stanford.edu"

#########
#%setup
#########

##Just grabbing default packages from ubuntu repository
%post
	apt-get -ym update
	apt-get -ym install git libcgal-dev
    apt-get -ym install antlr libantlr-dev # ANTLR
    apt-get -ym install libcurl4-gnutls-dev libexpat1-dev libxml2-dev # DAP-prereqs (curl, expat XML parser)
    apt-get -ym install bison cmake flex gcc g++ # GNU toolchain
    apt-get -ym install gsl-bin libgsl-dev # GSL
    apt-get -ym install libnetcdf11 libnetcdf-dev netcdf-bin # netCDF and DAP
    apt-get -ym install libhdf5-serial-dev # HDF5
    apt-get -ym install ncl-ncarg # ESMF_RegridWeightGen (for ncremap)
    apt-get -ym install udunits-bin libudunits2-0 libudunits2-dev # UDUnits
    apt-get -ym install libcgal-qt5-dev
    apt-get -ym install libatlas-base-dev libsuitesparse-dev
    apt-get -ym install nco

%environment
	export IMAGE_NAME="NCO"
