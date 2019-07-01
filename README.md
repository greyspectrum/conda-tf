# conda-tf

This Dockerfile will build a containerized conda environment with Python, R, and Tensorflow, among other packages.

## Building

To run this container on a high performance computing cluster, you will need to build it locally, as a Singularity image.

First, [install Singularity](https://sylabs.io/guides/3.2/user-guide/installation.html) on a system where you have root privileges.

Then, install [Docker](https://docs.docker.com/install/).

Finally, build a Singularity container from the Dockerfile in this repo using [docker2singularity](https://github.com/singularityware/docker2singularity).
