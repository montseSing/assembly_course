Bootstrap:docker  
From:ubuntu:16.04

%post
    apt-get update
    apt-get -y install wget
    wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh -O miniconda.sh
    bash miniconda.sh
    conda config --add channels defaults
    conda config --add channels conda-forge
    conda config --add channels bioconda
    conda install --yes megahit
    conda install --yes prokka
    rm miniconda.sh
