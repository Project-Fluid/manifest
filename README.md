![Fluid Banner](https://raw.githubusercontent.com/Project-Fluid/manifest/fluid-10/fluid.png)

Fluid
===========
Project Fluid is an attempt to make android experience much better and different from the regular AOSP standard.
We are very thankful to everyone else who helped Fluid. This a new User Experience and we hope you enjoy using Fluid!

#FeelsFluid 

Credits
-------
* [**TeamSubstratum (Theme Engine)**](https://github.com/Substratum)
* [**LineageOS/Cyanogenmod**](https://github.com/LineageOS)
* [**MagmaProject**](https://github.com/MagmaProject)
* [**Yodita**](https://gitlab.com/yodita)
* [**ExtendedUI**](https://github.com/Extended-UI)

# Setting up Fluid source

To begin with you first have to initialize the repo:

```bash
repo init -u https://github.com/Project-Fluid/manifest.git -b rebase
```

Then sync it up:

```bash
repo sync --force-sync --no-tags --no-clone-bundle -j$(nproc --all)
```

<b>Note: 
- You must have atleast 120-150GB free space on your disk 
- Basic git knowedge</b>

Building Fluid
==================

```bash
. build/envsetup.sh && brunch device-codename
```
