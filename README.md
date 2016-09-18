# wine-lpa

This repo contains Archlinux source packages and patchwork for Wine-lpa. Additionally, the repo contains backups, as well.

As of Wine-1.9.18, I decided to switch and use wine-staging as a base. It's got some nice extra features and it has wine-rt support -I'v added back the printf messages of wine-rt, so that I can see when threads are mapped to FIFOs/rtprios. Some examples of stuff that I have added; 'pipe synchronization optimization patch', a number of hacks for installers or fixing minor issues in VSTs, fixes to mciseq, a few patches to silence noisy 'fixme' messages, a hack on pulseaudio to support 16 audio channels, etc...

The current most source package pulls from wine-git, then wine-staging (github) and then applies all of the staging patchwork... Follwing that, it then applies all of my additional patches; which have all been re-based to work with wine-staging.
