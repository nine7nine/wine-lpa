# wine-lpa

Backup for wine-lpa patchwork and archlinux pkgbuilds (and some unused (or borked) patches, not to be applied).

Wine is currently (at the time of this writing) at version 1.9.18 and wine-staging has integrated wine-rt and has a form of shared memory in wineserver, so I think most people who are using wine, would probably be using wine-staging to get all of the extra features that haven't landed upstream yet.

However, I tend to add aditional patchwork to work around issues that I encounter or add aditional features, if needed. I also tend to test and play with non-standard configurations. I've sourced patches from various versions of wine, one-offs needed to make xyz app work and additionally have added my own hacks...

Currently, there are several source packages in this repo for Archlinux. In each folder (named by wine version), aside from the pkgbuilds, exists the patchsets - although, each folder ocntains what sometimes appear to be the same patches; they often aren't, but may be revisions or versions that only apply over the wine-version of that folder.

There is also a source package for wine-staging-git. This source package pulls wine-staging's git branch, wine-git and then applies all of the wine-staging patches over wine-git sources... After this, I then apply the patches in the PKGBUILD (minus, one's that are commented out (for now, or to be removed later).
