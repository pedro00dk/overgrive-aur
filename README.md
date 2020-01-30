# OverGrive AUR build script

![Auto-update](https://github.com/pedro00dk/overgrive-aur/workflows/Auto-update/badge.svg)

AUR: https://aur.archlinux.org/packages/overgrive/

This repository provides an easy way to install OverGrive in arch+based distributions.
The generated package through the command `makepkg` does not contain any OverGrive source code. Therefore, it is only a build script.


The OverGrive site already provides a ```tar.xz``` package. However the provided package is not in the AUR and requires extra steps before and after the package installation.
This package downloads the one obtained from the OverGrive site as base, and executes the necessary steps to make it work without any extra steps.

This repository uses github actions to automatically check the current available version in the [overgrive website](https://www.thefanclub.co.za/overgrive) and automatically updates itself when a new version is released.

Manual intervention is still required to update the AUR version. (Check TODO in auto-update.yml workflow).

Use ```sh build.sh``` to test the build and generate the ```.SRCINFO```
