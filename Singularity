
# FMRIPREP from poldracklab

BootStrap: docker
From: poldracklab/fmriprep:latest

%runscript
    exec /usr/local/miniconda/bin/fmriprep "$@"
    
%environment

%post
    #------------------------------------------------------------------------------
    # Create local binding points for our ICS-ACI
    #------------------------------------------------------------------------------
    mkdir -p /scratch
    mkdir -p /data
