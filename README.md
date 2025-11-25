The rule file is for disabling keyboard event from Lenovo mouse K91 on Linux.
Linux does not have driver to handle the DPI button event from the device and
the system will behavior unexpectly.

How to activate the rule?<br>
 sudo cp ./99-k91-disable-keyboard.rules /etc/udev/rules.d/<br>
 sudo udevadm control --reload<br>
 sudo udevadm trigger<br>

When you press down the DPI button, the mouse still freezes for a moment, it is
normal.
