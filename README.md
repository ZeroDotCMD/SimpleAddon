Install quick start macros 
SSH into your printer and run this command to copy Quick Start and Eddy calibration to your install.

```
wget -O /usr/data/printer_data/config/simpleaddon/eddycalibrate.cfg https://raw.githubusercontent.com/ZeroDotCMD/test/main/eddycalibrate.cfg
wget -O /usr/data/printer_data/config/simpleaddon/quickstart.cfg https://raw.githubusercontent.com/ZeroDotCMD/test/main/quickstart.cfg
sed '12i [include quickstart.cfg]
13i [include eddycalibrate.cfg]' /usr/data/printer_data/config/printer.cfg > /usr/data/printer_data/config/temp.cfg && mv /usr/data/printer_data/config/temp.cfg /usr/data/printer_data/config/printer.cfg

```


