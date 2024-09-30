# SimpleAddon for SimpleAF
SimpleAddon adds a few extra helpful options for SimpleAF. Included addons are listed bellow


Auto Save Z Offset - Automatically saves gcode_z_offset into a variables files each time a change is made and auto loads z_offset on startup.

Probe calibration - Dialog window for easier probe setup

Quick Start - Automate basic printer calibration




# Install
SSH into your printer and run the command that matches your probe.



# SimpleAddon for BTT Eddy

```
mkdir -p /usr/data/printer_data/config/simpleaddon
wget -O /usr/data/printer_data/config/simpleaddon/eddycalibrate.cfg https://raw.githubusercontent.com/ZeroDotCMD/SimpleAddon/configs/main/eddycalibrate.cfg
wget -O /usr/data/printer_data/config/simpleaddon/quickstart.cfg https://raw.githubusercontent.com/ZeroDotCMD/SimpleAddon/configs/main/quickstart.cfg
wget -O /usr/data/printer_data/config/simpleaddon/autozoffset.cfg https://raw.githubusercontent.com/ZeroDotCMD/SimpleAddon/configs/main/autozoffset.cfg
sed -i '12i [include simpleaddon/quickstart.cfg]\n\n[include simpleaddon/eddycalibrate.cfg]\n\n[include simpleaddon/autozoffset.cfg]' /usr/data/printer_data/config/printer.cfg

```


