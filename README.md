# Easybuild recipe for the NVHPC compilers

## Set up easybuild

On maui-ancil, 
```
module load Python
pip install easybuild --user
```

You can check the installation with
```
module purge
module load Easybuild
module list
eb --version
```

To upgraded to the latest easybuild,
```
pip install --upgrade easybuild
```

## How to build the recipe

```
module load Easybuild
eb NVHPC-24.3-CUDA-12.2.2.eb --robot --accept-eula-for=CUDA
```
