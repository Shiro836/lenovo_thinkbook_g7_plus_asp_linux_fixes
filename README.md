# lenovo_g7_plus_asp_linux_fixes
fixes for touchpad, bluetooth and suspend for lenovo 14/16 g7+ ASP 

# Touchpad
## Fix:
Compile libinput from sources

# Bluetooth
## Fix:
Update kernel to 6.12+ and execute this:
```bash
echo "0489 e111" | sudo tee /sys/bus/usb/drivers/btusb/new_id
```
"0489 e111" is taken from lsusb output

# Suspend
## Fix:
No fix yet, please help
