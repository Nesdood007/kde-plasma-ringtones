# KDE LMMS Competition Entries

These sounds were put together initially for the [KDE Plasma Mobile Audio Competition](https://community.kde.org/Promo/Plasma_Mobile_Audio_Competition). Please be sure to read the license section below if you decide to use these sounds or music in one of your projects.

## License

The sounds included in this repo are licensed as [CC-BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/).
A copy of the license text has been provided in the `LICENSE` file.

## Files included

__/project_files__
- All Project source files are included in here

__/keyboard_samples__
- All original unprocessed keyboard samples are here.

__/final_sounds/__

- __/keyboard__ - This is where the keyboard sounds are located. Plse see the Keyboard sounds section to learn more about how the files are named and how they are inteded to be used
- __/ringtones__ - This is where the ringtones are located. There is not really any distinction between which ones are alarms and which ones are ringtones, as I imagine that people will end up using sounds like these for both categories.
    - See the __Looping__ section to learn more about which sounds are able to be looped
- __/alerts__ - This is where the alert sounds are located. These are short sounds that are for system events, or for incoming SMS messages
- __/alarms__ - This is where the alarm sound is. This sound is loopable.

### Keyboard Sounds

I included sounds for modifier keys, the space bar, and normal keys. They are located in the `/final_sounds/keyboard` directory, and named using the following schema:

`<prefix><number><suffix>`

Where the prefix is one of:

- `s` for the Space bar
- `n` for a normal key
- `m` for a modifier key
- `b` for the backspace key

and Where the number is the sample number

and Where the suffix, if any, is:

- `p` - Downpress of a key
- `r` - Release of a key

The idea here is to provide a small variety of sounds such that any key can be pressed consecituvely and not have the same sound. For example, if I pressed a normal key, say the letter A, and then hit the letter S key, the sounds played could be n1.wav and then n2.wav, so that you hear a similar bit not quite the same sound. Now, if the user decided to press the Control key, they would normally hold it down before pressing any other key, so I split the sounds up into a downpress sound that would be played when the user hit the key initially, and then another sound that would be played when the user would release the key. Lastly, I provided sounds for the space bar abd the backspace keys, since they have distinct sounds on the keyboard.

## Looping

The following ringtones are loopable:
- Ringtone 1 (`r1.wav`)
- Ringtone 2 (`r2.wav`)
- Ringtone 3 (`r3.wav`)
- Ringtone 6 (`r6.wav`)
- Ringtone 7 (`r7.wav`)
- Ringtone 8 (`r8.wav`)
- Ringtone 9 (`r9.wav`)
- Ringtone 10 (`r10.wav`)
- Ringtone 11 (`r11.wav`)

Each of those ringtones are repeated twice so that the ring from the reverb is present in the second iteration of the loop.

The rest of the ringtones (4, 5, and 12) are not loopable, but I made sure that the ends are properly faded out so that they can be repeated if necessary.

## Samples used

- Sonic Pi's Sample Library
    - See https://github.com/sonic-pi-net/sonic-pi/tree/main/etc/samples
    - Licensed as CC0
    - All drum samples come from here
- Salamander Piano
    - https://sfzinstruments.github.io/pianos/salamander
    - CC-BY-3.0
    - Used for some of the system event / SMS sounds, and an alarm sound
- Samples I recorded from my IBM Model M Keyboard
    - These are licensed the same way as the rest of the resources in this repo

## Tools used
- LMMS
- Audacity was used to cut down the exported audio tracks and properly fade out the reverb ring at the end
    - For the keyboard typing noises, Audacity was used to record the keyboard sounds, and cut them apart to be used in LMMS, where a hard gate effect was applied