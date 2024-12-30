# lenovo_thinkbook_g7_plus_asp_linux_fixes
fixes for touchpad, bluetooth and suspend for Lenovo Thinkbook 14/16 g7+ ASP 

# Touchpad
## Fix:
Compile libinput from sources
https://wayland.freedesktop.org/libinput/doc/latest/building.html

# Bluetooth
## Fix:
Update kernel to 6.12+ and execute this:
```bash
echo "0489 e111" | sudo tee /sys/bus/usb/drivers/btusb/new_id
```
"0489 e111" is taken from lsusb output

# Suspend
## Fix:
https://4pda.to/forum/index.php?showtopic=1083187&view=findpost&p=134008907 - use translator

https://github.com/ty2/ideapad-laptop-tb2024g6plus
adjust hardware UUIDs using dmidecode

# Hibernate
## Fix:
no known fix, just turn it off I guess
