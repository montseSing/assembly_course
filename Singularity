Bootstrap:docker
From: continuumio/miniconda3:4.4.10

%environment
    export PATH="/opt/conda/bin:/usr/local/bin:/usr/bin:/bin:"
    unset CONDA_DEFAULT_ENV
    export ANACONDA_HOME=/opt/conda

%post
    export PATH=/opt/conda/bin:$PATH
    conda config --add channels defaults
    conda config --add channels conda-forge
    conda config --add channels bioconda
    conda install --yes megahit=1.2.9=hfbae3c0_0
    conda install --yes prokka
