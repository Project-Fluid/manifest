# Syncing Fluid

To begit with you first have to initialize:

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
