
### development history - problem summary

MacBook Air (Retina, 13-inch, 2019)
using an Apple USB-C to HDMI converter amd a KLAU 4 port HDMI kvm.

When using my macbook air in "clamshell" mode and with the kvm, it always reverts to a static "snow" screen, and I'd need to either re-plug the hdmi cable / adapter, open the laptop lid and close it back, or restart the laptop to get the display back.

I found that resetting the screen resolution 720p and back to 1080p will also fix the issue... but needed a way to programatically call the display changes since it's kind of hard to see where your mouse is when your screen is all snow.

### development history - solution (work-around) summary

Found display manager and installed it. 
After that all that's needed is an automator task and keyboard shortcut to execute:

```console
python /usr/local/bin/display_manager.py res 1280 720 60 main
python /usr/local/bin/display_manager.py res 1920 1080 60 main
```

![setup quick action](https://github.com/thomstratton/harp-screenFix/blob/main/set%20up%20automator%20quick%20action%20-%201.png?raw=true)
