This Patch is part of the [TESSER environment](https://bitbucket.org/AdrianArtacho/tesserakt/src/master/).

![TTESS:Logo](https://bitbucket.org/AdrianArtacho/tesserakt/raw/HEAD/TESSER_logo.png)

# Tesser_delay

This device takes a midi input and delays it by an anount of time that can be fix (in milliseconds) or proportional to the current tempo

![TESS:delay](https://docs.google.com/drawings/d/e/2PACX-1vSY5tPxPJAz-e3lKP6LcjSKrl4MXBU2I3c-ekQ02EicnxON9fFMW7IFgdhEzwGuT2PW1UqeSH9ifO5r/pub?w=715&h=350)

<sup>View of the device. Click  [here](https://docs.google.com/drawings/d/1PhLockgp09icAxNFx-1PHGeKwntM-sPB3hn-L10hLMU/edit) to edit.</sup>

### Usage

* Quick summary
* Version
* [Learn Markdown](https://bitbucket.org/tutorials/markdowndemo)

### Preset grid

The 10x10 grid in the center of the device can store a maximum of 100 different presets, including the *Thu/Mirror* toggles and the *VelRange* maximum reduction percent.

`mouse Click` recalls a preset (also CC21)

`SHIFT + mouse Click` stores a preset within the device/set.

### Save settings as an external file

The settings can be stored ina a human-readable file for reference. Here's a description of the button's dunctions on the right-hand side of the device:

`autoload` By clicking on *autoload* you can set (and store) the path to the file whose preset you wish to load on startup. By hovering over it with the mouse, you can see the path to the currently set file on the *Info View* window in Live.

`read` / `write` These buttons reads or write the contents of/from a *.txt* file.

`SAVE` The button *SAVE* amounts to *writeagain*, and causes the current settings to overwrite the ones in the loaded settings file.

`values` The button *values* amounts to *clientwindow*, and shows the values stored with the device/set.

____

# To-Do

* Document features
* Tesser_delay: just put a Toggle on each tesser delay line and save the settings
* Have only 1 delay line per device (or toggle of the other ones)
* have delay values "mappable", so that I can store them in clips as automation data
* make <Tesser_delay> microtone-polyphony-capable (speak seamlessly with gt_Transmitter)
* didn't I use the OSC adress 7533 already? what for? re-purpose
* pipe ALL midi messages, so that it can be used to delay CC as well...
* ZEITLUPE (vs. 'linear' delay) modi<> Tesser_delay modi: ABSOLUTE (saved, automation, CC), RELATIVE (to current transport tempo), SYNCED (to beat grid), DYNAMIC (Velocity dependant?)
* ...for "DYNAMIC" modus of [Tesser_delay] we need to know which is the 1st note.  We could do that by pulling a "gesture Start/End" message.
* add FB (feedback) knob... ( the highest position would be an infinite delay)
* ...have "bouncy balls" initiate the "gesture" starting in different places.  ....bouncy ball + scale....
* swap `factor` and `semitones` GUI
* **deprecate** active toggle
*  
