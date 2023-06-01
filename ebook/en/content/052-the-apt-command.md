
# The `apt` command

`apt`(Advantage package system) command is used for interating with `dpkg`(packaging system used by debian). There is already `dpkg` command to manage `.deb` packages. But `apt` is more user-friendly and efficient way.
	
In simple terms `apt` is a command used for installing, deleting and other operations on debian based Linux.
	
You will be using `apt` command mostly with `sudo` privileges.

### Installing packages:
`install` followed by `package_name` is used with `apt` to install new package.
##### Syntax:
```
sudo apt install package_name
```
##### Example:
```
sudo apt-get install g++
```
This command will install g++ on your system.


### Removing packages:
`remove` followed by `package_name` is used with `apt` to remove specific package.
##### Syntax:
```
sudo apt remove package_name
```
##### Example:
```
sudo apt-get remove g++
```
This command will remove g++ from your system.


### Removing unused packages:
Whenever a new package that depends on other packages is installed on the system, the package dependencies will be installed too. When the package is removed, the dependencies will stay on the system. This leftover packages are no longer used by anything else and can be removed.

##### Syntax:
```
sudo apt autoremove
```
This command will remove all unused from your system.


### Updating package index:
`apt` package index is nothing but a database that stores record of available packages that are enabled on your system.

##### Syntax:
```
sudo apt update
```
This command will package index on your system.


### Upgrading packages:
If you want to install latest update for your install packages you may wanna run this command.
##### Syntax:
```
sudo apt upgrade
```
The command doesn’t upgrade packages that require removal of installed packages.

If you want to upgrade a single package, pass the package name:
##### Syntax:
```
sudo apt upgrade package_name
```
This command will upgrade your packages to latest version.


