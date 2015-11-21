# pulseaudio-systemd

This is a systemd service to run pulseaudio in system-wide mode.

Running pulseaudio in system-wide mode is generally a bad idea and shouldn't be done unless required.
Read [this](http://www.freedesktop.org/wiki/Software/PulseAudio/Documentation/User/WhatIsWrongWithSystemWide) for more 
information.

Instructions
-------
1. Clone the repository
2. $ makepkg
3. # pacman -U *.xz
4. Add the user and root to the "pulse-access" group
5. # systemctl enable pulseaudio
6. Disable pulseaudio autostarting by the Desktop Environment.
7. Reboot

Credits
-------
Dmitry Fillo, Joseph Lehner

