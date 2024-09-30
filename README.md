Install quick start macros 
SSH into your printer and run this command to copy Quick Start to your install.

```
wget -O /usr/data/printer_data/config/quickstart.cfg https://raw.githubusercontent.com/ZeroDotCMD/test/main/quickstart.cfg
echo "[include quickstart.cfg]" | cat - /usr/data/printer_data/config/printer.cfg > /usr/data/printer_data/config/temp.cfg && mv /usr/data/printer_data/config/temp.cfg /usr/data/printer_data/config/printer.cfg

```


