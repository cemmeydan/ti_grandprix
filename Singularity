#######################################################################################
## DO NOT EDIT THIS FILE! This file was automatically generated from the dockerfile. ##
## Run dynwrap:::.container_dockerfile_to_singularityrecipe() to update this file.   ##
#######################################################################################

Bootstrap: shub

From: dynverse/dynwrap:py3.6

%labels
    version 0.1.1

%post
    chmod -R a+r /code
    pip install tensorflow
    git clone https://github.com/GPflow/GPflow.git && cd GPflow && pip install GPflow
    git clone https://github.com/ManchesterBioinference/GrandPrix && cd GrandPrix && python setup.py install

%files
    . /code

%runscript
    exec python /code/run.py

