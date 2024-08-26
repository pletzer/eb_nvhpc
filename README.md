# Easybuild recipe for the NVHPC compilers

## How to build the recipe

on maui-ancil
```
module load Easybuild
export EASYBUILD_MODULES_TOOL=EnvironmentModulesC
export EASYBUILD_MODULE_SYNTAX=Tcl
eb NVHPC-24.7-CUDA-12.2.2.eb --robot --accept-eula-for=CUDA
```
