# wine-lpa

This repo contains Archlinux source packages and patchwork for Wine-lpa. Additionally, the repo contains backups, as well.

As of Wine-1.9.18, I decided to switch and use wine-staging as a base. It's got some nice extra features and it has wine-rt support ~ I decided to add back the printf messages of wine-rt, so that I can see when threads are mapped to FIFOs/rtprios. 

Some examples of stuff that I have added from wine-lpa; 'pipe synchronization optimization patch', a number of hacks for installers, fixing minor issues/bugs with VSTs, fixes to mciseq, a few patches to silence noisy 'fixme' messages that spam a terminal or winedebug, a hack on pulseaudio to support 16 audio channels, etc, etc...

The moust current source package pulls from wine-git, then wine-staging (github) and then applies all of the staging patchwork... Follwing that, it then applies all of my additional patches; which have all been re-based to work with wine-staging.
