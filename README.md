# pulseaudio-headphone-config

These config files will split the lineout and headphone ports on the same sink in PulseAudio. By default, when headphones are plugged in, the lineout is muted. If lineout is unmuted (by disabling automute) then both headphones and lineout start playing sounds.

From https://wiki.archlinux.org/index.php/PulseAudio/Examples#Having_both_speakers_and_headphones_plugged_in_and_switching_in_software_on-the-fly

## To use:
* Take backups of /usr/share/pulseaudio/alsa-mixer/paths/analog-output-lineout.conf and ....headphones.conf
* Clone this repo to a folder
* Copy the conf files in this repo to the /usr/share/pulse.....paths/ directory
* run alsamixer -c0 and disable automute
* Restart pulseaudio service

### Tested on:
Fedora 32 (kernel 5.8.10); pulseaudio 13.99.1-rebootstrapped, Asus Strix Motherboard with Realtek ALC1220 soundcard
