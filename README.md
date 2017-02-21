blackfuel / asuswrt-merlin-addon
================================

Compile your own pre-built apps into the firmware image for high availability purposes or other reasons where it does not make sense to run the app from an external USB storage device.  

For example, Dnscrypt is an app that performs DNS lookups and it should be compiled into the firmware, since without it, LAN clients would not be able to access the Internet.  Another example is Cryptsetup because it cannot be installed on an encrypted USB storage device when it's the program used to mount the encrypted USB storage device.  

Any pre-built app may be compiled into the firmware image.  This allows you to run any Entware, Optware or Asuswrt-linked app side-by-side within the firmware. And since the firmware is squashfs compressed, all of your pre-built apps are safely and securely compressed into the read-only firmware image.  

The technique for doing this is a set of tools that change the library root folder for each selected program and its dependencies, from "/opt" to "/entware", "/optware", "/native", or some other root folder name.


#### Donations: Any amount will help.  Thank you.
Bitcoin: 1i5Tpno73gJdr1XdmoxT6CjVFGef5KkZM
