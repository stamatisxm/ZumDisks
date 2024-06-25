# ZumDisks
Zenity Assisted Mount / Unmount Devices

<img alt="ZumDisks Logo" src="http://ideaware.stamatis.uk/wp-content/uploads/2016/01/ZumDisks.png" width="48px" height="48px" />

## ZumDisks – { Mount / Unmount Block Devices }
ZumDisks is a simple Zenity front-end to udisks and udisksctl, useful for handling the mounting / unmounting of partitions on internal and removable disks. The interface is simple and self explanatory.

### { Program Options }

This is the interface of ZumDisks:

<img alt="ZumDisks Interface" src="http://ideaware.stamatis.uk/wp-content/uploads/2016/01/ZumDisks-SShot.png" />

The “Mountable Devices” is a drop-down that displays the partitions (internal and removable) that can be mounted at runtime. To mount a device select it from the drop-down and click on the “Mount/Unmount/Refresh” button.

The “Mounted Devices” displays a list of devices currently mounted.

The “Unmountable Devices” is a drop-down that displays the partitions that can be unmounted at runtime. To unmount a device, select it from the drop-down and click on the “Mount/Unmount/Refresh” button.

NOTE: System partitions (/, /home, /usr, /tmp, etc) are NOT available in this drop-down menu, as they may NOT be unmounted at runtime.
Lastly, there is a help drop-down menu, labelled “Click drop-down Help”, summarizing the program’s operation.



### { Program Setup }
This program is going to be installed by default in your **$HOME/bin** directory. If you have not set your **$HOME/bin** in the **$PATH**, see [this](http://istos.stamatis.uk/linux/include-homebin-in-any-desktop-environment/ "Include $HOME/bin in any Desktop Environment") or [this snippet](http://istos.stamatis.uk/linux/include-homebin-in-the-path-for-bash-shell "Setup your $HOME/bin in the $PATH") for details.

To run this program, you need to have the following packages installed in your system (Check with your package manager):

- _**zenity**_
- _**sudo**_
- Either _**udisks**_ or _**udisks2**_ (or both)

#### Once the above packages are installed
- Download ZumDisks
- Move the downloaded tarball into your **$HOME**, as all extracted files and directories will be relative to your **$HOME**
- Expand the tar file in a terminal by issuing:  
<code>**tar xf ZumDisks\_&lt;version&gt;.tar**</code>
- Invoke the program from the terminal, running:  
<code>**ZumDisks &**</code>  
to ensure that it loads properly and no error messages are shown.

If everything has gone ok, you should be able to find the program in the _**Accessories**_ program group on your desktop manager.

### { File List }
The tarball contains these files (relative to the user's $HOME):
<pre>
bin/ZumDisks
.local/share/icons/ZumDisks.png
.local/share/applications/ZumDisks.desktop
</pre>

