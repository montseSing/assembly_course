Bootstrap:docker  
From:continuumio/anaconda

%environment
    export PATH="/opt/conda/bin:/usr/local/bin:/usr/bin:/bin:"
    unset CONDA_DEFAULT_ENV
    export ANACONDA_HOME=/opt/conda

%post
    export PATH=/opt/conda/bin:$PATH
    conda config --add channels defaults
    conda config --add channels conda-forge
    conda config --add channels bioconda
    conda install --yes megahit
    conda install --yes prokka
