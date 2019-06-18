
# FMRIPREP from poldracklab

BootStrap: docker
From: poldracklab/fmriprep:latest

%runscript
    exec /usr/local/miniconda/bin/fmriprep "$@"
    export FMRIPREP_DIR=/usr/local/miniconda/bin
    export space_variant=MNI152NLin2009cAsym
    
%environment

%post
    #------------------------------------------------------------------------------
    # Create local binding points for our ICS-ACI
    #------------------------------------------------------------------------------
    mkdir -p /scratch
    mkdir -p /data
