# HotCorner for Windows 10

![HotCorner Logo](https://github.com/kowalski7cc/hotcorner/blob/master/Resources/HotCorner.png)

This is the same app from [Taviso's Tiny Hot Corners](https://github.com/taviso/hotcorner), but packaged for Windows 10!

In GNOME 3 whenever you move the mouse to the top left corner, GNOME switches to the activities view.
Whenever I'm using Windows 10, I always forget that this doesn't work. Bleh.

I searched around for existing solutions, and wasn't happy with anything I could find.

The options seem to be

* Some ridiculous AutoHotKey monstrosity (?!?).
* Massive Delphi application with 100MB of resources.
* Some naive program that polls GetCursorPos() in a busy loop.

None of these are what I want, I just want that GNOME 3 thing with absolute minimal overhead.

This is a **very** minimal hotcorner app, written in C.
You can adjust parameters, delays, bindings easily and recompile.

Zero state is stored anywhere, no registry keys or configuration files.

* If you want to configure something, edit the code and recompile.
* If you want to uninstall it, just uninstall it like any other UWP app.

## Install and build instructions

[Downloads link](https://github.com/kowalski7cc/HotCorner/releases)
Download Appx, add [certificate](https://stackoverflow.com/questions/23812471/installing-appx-without-trusted-certificate) to your system and install or load solution and run distribution.

### Uninstalling

You can uninstall HotCorner like any other UWP app.
If you want you can disable autostart from TaskManager.

## License

GPL3

## Authors

* Kowalski7cc [@kowalski7cc](https://github.com/kowalski7cc/) - Appx migration
* Tavis Ormandy [@taviso](https://github.com/taviso/) - Original Author
* Ahmed Samy [@asamy](https://github.com/asamy) - HotKey support

## FAQ

* Q: I don't want to compile it, can't you just give me a prebuilt version? :(
* A: Checkout the releases, [here](https://github.com/kowalski7cc/HotCorner/releases).

* Q: Can you change a setting, and then compile it for me?
* A: No.

* Q: How do I turn it off without rebooting?
* A: Use task manager to kill HotCorner process.