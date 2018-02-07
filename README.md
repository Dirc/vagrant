# Vagrant files

# Remarks:
## Resolve rsync error
Error message: rsync could not be found in path
Solution: install mingw

To install MinGW:
1. Goto MinGW mother site at http://www.mingw.org/  Downloads  Installer  click on "mingw-get-inst" link to download the installer.
2. Run the downloaded installer.
  * Set the installation directory. (Try to use a directory name without spaces, e.g., "d:\myproject\mingw". Try not to install under "Program Files" or "Desktop".)
  * All Packages > MSYS > MSYS System Builder > search for rsync packages (3)
  * In MinGW Installation Manager, select "Installation"  "Update Catalogue"  Select all packages in "Basic Setup"  continue.
3. Setup environment variable PATH to include "<MINGW_HOME>/bin" where <MINGW_HOME> is the MinGW installed directory that you have chosen in the previous step.

## Resolve VirtualBox guest additions error
```text
vagrant plugin install vagrant-vbguest
```
