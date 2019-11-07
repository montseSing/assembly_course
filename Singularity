Bootstrap:docker
From: ubuntu:16.04

%files
    Miniconda2-latest-Linux-x86_64.sh
%post
    bash Miniconda2-latest-Linux-x86_64.sh
    conda config --add channels defaults
    conda config --add channels conda-forge
    conda config --add channels bioconda
    conda install --yes megahit
    conda install --yes prokka
