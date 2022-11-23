# apple-scripts
Usefull apple scripts

![Usefull apple scripts](/assets/apple-script.gif "How to run it")


# [Copy to Clipboard](/Copy%20to%20Clipboard.scpt)
```applescript
set the clipboard to "Lorem ipsum dolor sit amet, consectetur adipiscing elit."
```

# [Scrcpy Open](/Scrcpy%20Open.scpt)
```applescript
# DEVICE_SERIAL_NUMBER: run "adb devices"

tell application "Terminal"
	
	activate
	
	do script "scrcpy -s DEVICE_SERIAL_NUMBER -w" in front window
	
end tell
```

# [Scrcpy Record](/Scrcpy%20Record.scpt)
```applescript
# DEVICE_SERIAL_NUMBER: run "adb devices"

tell application "Terminal"
	
	activate
	
	do script "scrcpy -s DEVICE_SERIAL_NUMBER -w -t -b2M -m800 -r $HOME/Desktop/file.mp4" in front window
	
end tell
```

# Reference

* [scrcpy](https://github.com/Genymobile/scrcpy): This application provides display and control of Android devices connected via USB or over TCP/IP. It does not require any root access. It works on GNU/Linux, Windows and macOS.

* [adb](https://developer.android.com/studio/command-line/adb?gclid=CjwKCAiApvebBhAvEiwAe7mHSJI_Rq0EAaJ8aZyt--E7Wsnxb7-9idbgKLZTP0qne0Eo2bzGzRnR4hoCXe4QAvD_BwE&gclsrc=aw.ds): Android Debug Bridge (adb) is a versatile command-line tool that lets you communicate with a device. The adb command facilitates a variety of device actions, such as installing and debugging apps, and it provides access to a Unix shell that you can use to run a variety of commands on a device.