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

Contributing
===============

To contribute to fluid you can use our gerrit (https://review.projectfluid.org)
Let's imagine you haven't used gerrit, this will teach you how to use it.

Clone any repo from our github, for example, settings app:
```bash
git clone https://github.com/Project-Fluid/packages_apps_Settings settings
```

Sign into gerrit using the sign in button on the top right

Then generate a ssh key (if you already generated one, skip this step):
```bash
ssh-keygen -o
```

And add your public ssh key (by default located in ~/.ssh/id_rsa.pub) to your gerrit profile (https://review.projectfluid.org/settings/#SSHKeys)

After that, do your changes and commit them:
```bash
git commit
```

And finally, push the changes (this is an example for settings with the default fluid-11 branch, you can replace the repo part with any other repo you would push):
```bash
git push "ssh://YOURUSERNAME@review.projectfluid.org:29418/Project-Fluid/packages_apps_Settings" HEAD:refs/for/fluid-11
```
NOTE: If you do get an error telling you to run a command and then amend the commit, do it, then retry to push.
