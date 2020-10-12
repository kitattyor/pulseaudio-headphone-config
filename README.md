# pulseaudio-headphone-config

Adapted from https://wiki.archlinux.org/index.php/PulseAudio/Examples#Having_both_speakers_and_headphones_plugged_in_and_switching_in_software_on-the-fly

## To use:
* Take backups of /usr/share/pulseaudio/alsa-mixer/paths/analog-output-lineout.conf and ....headphones.conf
* Clone this repo to a folder
* Copy the conf files in this repo to the /usr/share/pulse.....paths/ directory
* run alsamixer -c0 and disable automute
* Restart pulseaudio service
