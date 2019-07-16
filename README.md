# conda-tf

This Dockerfile will build a containerized conda environment with Python, R, and Tensorflow, among other packages. Additionally, a Singularity deifinition file is included, which will build a conda environment from any `environment.yml`, specified at build time.

## Building

To run this container on a high performance computing cluster, you will need to build it locally, as a Singularity image.

First, [install Singularity](https://sylabs.io/guides/3.2/user-guide/installation.html) on a system where you have root privileges.

Then, install [Docker](https://docs.docker.com/install/).

To build a Singularity container from the Dockerfile in this repo, use [docker2singularity](https://github.com/singularityware/docker2singularity).

To build from the Singularity definition file included in this repo directly, first export the Conda environment you wish to define for your container:

`conda env export > environment.yml`

Then build the Singularity image, with your environment.yml in the same directory:
