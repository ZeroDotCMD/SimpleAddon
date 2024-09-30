# SimpleAddon for SimpleAF
SimpleAddon adds a few extra helpful options for SimpleAF. Included addons are listed bellow


Auto Save Z Offset - Automatically saves gcode_z_offset into a variables files each time a change is made and auto loads z_offset on startup.

Probe calibration - Dialog window for easier probe setup

Quick Start - Automate basic printer calibration




# Install
SSH into your printer and run the command that matches your probe.



# SimpleAddon for BTT Eddy

```
mkdir -p /usr/data/printer_data/config/SimpleAddon
wget -O /usr/data/printer_data/config/SimpleAddon/eddycalibrate.cfg https://raw.githubusercontent.com/ZeroDotCMD/SimpleAddon/main/SimpleAddon/eddycalibrate.cfg
wget -O /usr/data/printer_data/config/SimpleAddon/quickstart.cfg https://raw.githubusercontent.com/ZeroDotCMD/SimpleAddon/main/SimpleAddon/quickstart.cfg
wget -O /usr/data/printer_data/config/SimpleAddon/autozoffset.cfg https://raw.githubusercontent.com/ZeroDotCMD/SimpleAddon/main/SimpleAddon/autozoffset.cfg
sed -i '12i [include SimpleAddon/quickstart.cfg]\n\n[include SimpleAddon/eddycalibrate.cfg]\n\n[include SimpleAddon/autozoffset.cfg]' /usr/data/printer_data/config/printer.cfg

```


