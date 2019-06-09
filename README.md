i3exit - Shut down/reboot from within i3.
===
Small GTK script allowing for shutting down/rebooting computer
from within i3. The script is written in Perl, and requires
the **Perl-GTK version 3** module to function. The script also
relies on **systemd** being used as init system.
<div style="text-align:center"><img src="https://i.imgur.com/WxP9Wa1.png" alt="i3exit"></div>

---
To use, simply clone this repository, make **i3exit** executable and
put it in a directory in your ``$PATH`` and set up a keybind in your
i3 config file, or modify the default keybind for exiting i3:

``bindsym $mod+Shift+e exec i3exit``

Then install the required Perl-GTK package:

Fedora:
``sudo dnf install perl-Gtk3``

Ubuntu:
``sudo apt install libgtk3-perl``

Arch Linux:
``sudo pacman -S perl-gtk3``

Finally, reload i3 with `Mod+Ctrl+e` and you should be good to go.
