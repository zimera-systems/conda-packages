# Conda Packages

This repo is used to store all metadata files for all conda packages at https://anaconda.org/zimera

## Packages Needed

2 packages should be installed using **conda**:

1.  conda-build
2.  anaconda-client

## Building 

1.  Enter directory
2.  ``conda build .``

The result will be in (example): ``$MINICONDA_HOME/envs/{{ env name }}/conda-bld/linux-64/nebula3-python-3.0.0-py310_0.tar.bz2``

## Re-building

To rebuild, delete ``conda-bld`` dir at your env, then ``conda build .``

## Convert to other platform

```
$ conda convert --platform all file.tar.bz2 -o outputdir/
```

## Upload

```bash
$ anaconda login

$ anaconda upload <file>
```
