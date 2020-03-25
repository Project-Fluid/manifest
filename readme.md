<p align="center">
<img src="https://raw.githubusercontent.com/Project-Fluid/manifest/fluid-10/fluid.png" width="800px" height="318.74px" > 
</p>

Fluid Q
===========
Project Fluid is an attempt to make android experience much better and different from the regular AOSP standard.
We are very thankful to everyone else who helped Fluid. This a new User Experience and we hope you enjoy using Fluid!

#stayfluid 

Credits
-------
* [**TeamSubstratum (Theme Engine)**](https://github.com/Substratum)
* [**LineageOS/Cyanogenmod**](https://github.com/LineageOS)
* [**Yodita**](https://gitlab.com/yodita)

# Setting up Fluid source

To begin with you first have to initialize the repo:

```bash
repo init -u https://github.com/Project-Fluid/manifest.git -b fluid-10
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
