
# Description

A collection of Fortran namelist i/o files, which contain the parameters for different runs of the radiation-MHD code Phab-C²

## Directory structure
    RUNSET/in/RUN.pars
Where `RUNSET` is `pdrturb`, `pdrkrum`, etc. 

## How to clone this repo into an existing directory tree

In my standard set-up, this directory structure is rooted in the directory `FOO/Fabio/C2Ray/runs/`, which also contains directories `RUNSET/out/`, which is where all the output datacubes go. Since the `runs/` directory already has things in it, we cannot do a `git clone git://github.com/deprecated/phabc2-runpars.git` into it. However, all is not lost since we can do the following:

    git init
    git remote add origin git://github.com/deprecated/phabc2-runpars.git
    git fetch # automaticlly creates * [new branch]      master     -> origin/master
    git add pdrturb/in/*.pars # adjust according to circumstance - must add all pre-existing files
    git checkout master



# Active run sets

## pdrturb

HII region in uniform magnetized medium. 

### Ostar-et
O star in turbulent medium, with entropy fix (`e`) and temperature ceiling (`t`), currently set at 3e4 K. 


## pdrkrum

HII region in turbulent, magnetized, molecular cloud

# Old run sets
