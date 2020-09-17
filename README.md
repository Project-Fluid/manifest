Fluid
===========
Project Fluid is an attempt to make the Android experience much better and different from the regular AOSP standard.
We are very thankful to everyone else who helped Fluid. This a new User Experience and we hope you enjoy using Fluid!

#FeelsFluid 

Credits
-------
* [**LineageOS**](https://github.com/LineageOS)

# Setting up Fluid source

To begin with you first have to initialize the repo:

```bash
repo init -u https://github.com/Project-Fluid/manifest.git -b fluid-11
```

Then sync it up:

```bash
repo sync --force-sync --no-tags --no-clone-bundle -j$(nproc --all)
```

<b>Note: 
- You must have at least 120-150GB free space on your disk 
- Basic git knowledge</b>

Building Fluid
==================

```bash
. build/envsetup.sh
lunch fluid_device-userdebug
mka bacon
```