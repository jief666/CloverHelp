# Do I have to share my serial number ?

Of course no !  
That said, I won't steal your serial number. Why would I ? They are free and I have mine since a long time.  
But better safe than sorry ? You're right.

You can :

### Remove

For working together, we don't need a serial number. Serial number will matter for iMessage and other things. Here, we're talking about booting macOS.  
Your serial number will be in the Clover folder you'll use every day, but not in this one.

### Externalize

Create a "smbios.plist" containing, for example :

```markup
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE plist PUBLIC "-//Apple//DTD PLIST 1.0//EN" "http://www.apple.com/DTDs/PropertyList-1.0.dtd">
<plist version="1.0">
<dict>
	<key>SMBIOS</key>
	<dict>
		<key>BoardSerialNumber</key>
		<string>your serial</string>
		<key>SerialNumber</key>
		<string>your serial</string>
		<key>SmUUID</key>
		<string>your uuid, if you have some</string>
	</dict>
</dict>
</plist>
```

Put this file in your daily Clover folder.

You can also put this file in the EFI we share. We already have added  `«CLOVER/smbios.plist»` to `«.gitignore»`, so not risk to share by mistake.  


_I would recommend to have a separate smbios.plist anyway. The big advantage is that you cannot share your serial number by mistake when you want to share your config.plist, on a forum for example._

