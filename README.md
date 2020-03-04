# HIGHLY EXPERIMENTAL, DO *NOT* USE !!!! (you have been warned, it might kill kittens !!!)

To use it anyway, take an Ubuntu Core 18 image, set it up and ssh in ... then:

```snap install mir-kiosk```

scp the ubuntu-core-desktop snap to it ....

then:

```
snap install --dangerous ubuntu-core-desktop_0.1_amd64.snap

snap connect ubuntu-core-desktop:account-control
snap connect ubuntu-core-desktop:hardware-observe
snap connect ubuntu-core-desktop:home
snap connect ubuntu-core-desktop:log-observe
snap connect ubuntu-core-desktop:login-session-control
snap connect ubuntu-core-desktop:login-session-observe
snap connect ubuntu-core-desktop:mount-observe
snap connect ubuntu-core-desktop:network-control
snap connect ubuntu-core-desktop:network-setup-control
snap connect ubuntu-core-desktop:physical-memory-observe
snap connect ubuntu-core-desktop:process-control
snap connect ubuntu-core-desktop:removable-media
snap connect ubuntu-core-desktop:shutdown
snap connect ubuntu-core-desktop:system-observe
snap connect ubuntu-core-desktop:x11-plug ubuntu-core-desktop:x11

```
