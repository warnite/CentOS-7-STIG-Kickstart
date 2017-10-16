CentOS 7 STIG Kickstart - Tested with 7.4

This is a kickstart with the goal of making CentOS 7 STIG compliant. I have been unable to find a working kickstart so I decided to make my own. This is still a WiP so feel free to improve or change anything.

This will currently perform a hands free install with an OpenScap score of 88%. The only additional packages installed not needed for STIG compliance are ClamAV, Libre-Office, XFCE, and OpenScap –Workbench.

Redacted Info

I have removed the --url and repo lines for my local mirrors. You will need to replace them with the base repo and epel repos for the install as it will pull the additional packages needed from there.

The kickstart will create a script in /root called RUN_AFTER_INSTALL.sh. This will prompt you to set the bootloader password, the root password, and the hostname.
