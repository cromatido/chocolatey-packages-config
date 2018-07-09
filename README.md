My Chocolatey Packages.config
=============================

To use this, you need to have [Chocolatey](http://chocolatey.org/) installed.

This could be done by issuing the following in a Command Prompt:

    @powershell -NoProfile -ExecutionPolicy unrestricted -Command "iex ((new-object net.webclient).DownloadString('https://chocolatey.org/install.ps1'))" && SET PATH=%PATH%;%systemdrive%\chocolatey\bin


Then get the packages.config file:

    curl -outfile packages.config https://raw.githubusercontent.com/cromatido/chocolatey-packages-config/master/packages.config
  
and now you're ready to install (might take some time):

    cinst packages.config
