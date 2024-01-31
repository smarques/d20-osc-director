notes:

RASPBERRY BOOKWORM

//if raspberry logsout when monitor goes to sleep

https://forums.raspberrypi.com/viewtopic.php?t=360888

It seems some monitors and kvms toggle hotplug when they shouldn't. You can disable hotplug detection by adding one of these option to the end of "/boot/firmware/cmdline.txt", this fixed my kvm issues:

    “vc4.force_hotplug=1” if using HDMI0
    “vc4.force_hotplug=2” if using HDMI1
    “vc4.force_hotplug=3” if using HDMI 0 and 1

This suggestion came from one of the Pi engineers viewtopic.php?p=2146832&hilit=waggle+hotplug#p2146832

LINKS

ARDOUR OSC: https://manual.ardour.org/using-control-surfaces/controlling-ardour-with-osc/osc-control/

