<p align="center">
<a href="https://www.arcade1up.com"><img style="text-align: center" width="500px" src="https://github.com/maddox/arcade1up-tools/raw/master/images/arcade1up-logo.png?raw=true" /></a>
</p>

<br>

This repo  collects a few things that are helpful for modding an Arcade1Up. If you're nostalgic and have played with emulation for a while, this is a great project. It's practically all just plug and play.


## Customization
* [Splash Screens](/splashscreens)
* [Images](/images)

## Resources
* [ETAPrime](https://youtube.com/etaprime)'s [amazing tutorial](https://www.youtube.com/watch?v=09DQCOr6zQM) modding an Arcade1Up with a Raspberry Pi and RetroPie
* [Arcade1Up Subreddit](https://reddit.com/r/arcade1up)
* [Retropie](https://retropie.org.uk)
* [Raspberry Pi Power Button Tutorial](https://gameroomsolutions.com/setup-daphne-raspberry-pi-3-retropie)
* [Raspberry Pi Volume Knob Tutorial](https://gist.github.com/savetheclocktower/9b5f67c20f6c04e65ed88f2e594d43c1)

## Parts

* [Raspberry Pi B+ & Power Adapter](https://amzn.to/2rLmCIR)
* [32GB SD Card](https://amzn.to/2CnEXSi)
* [LCD Controller Board](https://amzn.to/2GvkC1z)
* [Audio Amp](https://amzn.to/2Bz1CcH)
* [USB Replacement Buttons and Joystick](https://amzn.to/2LvsyPu) - Swap out your buttons easily. 
* [Competition Style Joystick Topper](https://amzn.to/2RbrNjC) - SF2 style sticks.
* [Rotary Encoder](https://amzn.to/2BwlIoc) - Use this for adding a volume knob to your cabinet.
* [Step bit](https://amzn.to/2Bxu6nv) - Use this to drill new holes in your cabinet for more buttons.
* [Master/Slave Power strip](https://amzn.to/2R5M2zm) - Plug your pi into `Master` and when it powers down, everything else powers down.

## Advanced RetroPie/Raspberry Pi Customizations

Here's some tricks of the trade to make your Arcade1Up mod look more official.

### Hide EmulationStation Splash screen

This disables EmulationStation's splash screen so that your custom splash screen shows until everything is completely booted up.

Edit `/opt/retropie/configs/all/autostart.sh` to be

    emulationstation --no-splash #auto

### Hide console output on boot

Edit `/boot/cmdline.text` and set `console=tty3`

### Hide Raspbery Pi Logo on boot

Edit `/boot/cmdline.text` and add `logo.nologo`
