#######################################################################################
## DO NOT EDIT THIS FILE! This file was automatically generated from the dockerfile. ##
## Run babelwhale::convert_dockerfile_to_singularityrecipe() to update this file.    ##
#######################################################################################

Bootstrap: shub

From: dynverse/dynwrap:py3.6

%labels
    version 0.1.7


    
    
    
    
    

%files

    . /code

%post
    mkdir /scratchLocal
    mkdir /pbtech_mounts
    mkdir /pbtech_mounts/softlib001
    mkdir /athena
    mkdir /zenodotus



    chmod -R 755 '/code'
    pip install tensorflow
    pip install git+https://github.com/GPflow/GPflow
    pip install git+https://github.com/ManchesterBioinference/GrandPrix

%runscript
    exec python /code/run.py

