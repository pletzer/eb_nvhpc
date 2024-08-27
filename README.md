# Easybuild recipe for the NVHPC compilers

## How to build the recipe

on maui-ancil
```
module purge
module load slurm NeSI EasyBuild
export EASYBUILD_MODULES_TOOL=EnvironmentModulesC
export EASYBUILD_MODULE_SYNTAX=Tcl

# stop after install step, required as a C++ 20 test is failing
eb NVHPC-24.7-CUDA-11.8.0.eb --robot --accept-eula-for=CUDA --stop install
```
