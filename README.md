# HCP Singularity Container

## Overview

This Singularity container is built for neuroimaging analysis, incorporating a variety of tools and libraries on Ubuntu 18.04. It includes ANTs, FSL, AFNI, Connectome Workbench, MRtrix3, FreeSurfer, and Matlab Runtime.

## Prerequisites

- Singularity
- Internet connection (for downloading packages)
- Freesurfer and Matlab Runtime packages in '/path/to/Singularity`

## Building the Container

1. Place `freesurfer-linux-ubuntu18_amd64-7.4.1.tar.gz` ([Download](https://surfer.nmr.mgh.harvard.edu/pub/dist/freesurfer/7.4.1/freesurfer-linux-ubuntu18_amd64-7.4.1.tar.gz)) and `runtime2014bLinux.tar.gz` ([Download](https://surfer.nmr.mgh.harvard.edu/fswiki/MatlabRuntime?action=AttachFile&do=get&target=runtime2014bLinux.tar.gz)) in `/path/to/Singularity`.
2. Use Singularity to build the container:
   ```bash
   sudo singularity build HCP Singularity.def

## Usage

Run the container using Singularity:
   ```bash
   singularity shell HCP
```

## Software Included

- **ANTs:** Image registration and segmentation.
- **FSL:** Analysis of FMRI, MRI, and DTI data.
- **AFNI:** Brain imaging data analysis.
- **Connectome Workbench:** Brain connectivity analysis.
- **MRtrix3:** Diffusion MRI data analysis.
- **FreeSurfer:** Neuroimaging data analysis.



