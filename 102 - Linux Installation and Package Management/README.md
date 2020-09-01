# Topic 102: Linux Installation and Package Management

## 102.1 Design hard disk layout
**Weight**: 2

**Description**: Candidates should be able to design a disk partitioning scheme for a Linux system.

Key Knowledge Areas:

- Allocate filesystems and swap space to separate partitions or disks.
- Tailor the design to the intended use of the system.
- Ensure the /boot partition conforms to the hardware architecture requirements for booting.
- Knowledge of basic features of LVM.

The following is a partial list of the used files, terms and utilities:

- / (root) filesystem
- /var filesystem
- /home filesystem
- /boot filesystem
- EFI System Partition (ESP)
- swap space
- mount points
- partitions

## 102.2 Install a boot manager
**Weight**: 2

**Description**: Candidates should be able to select, install and configure a boot manager.

Key Knowledge Areas:

- Providing alternative boot locations and backup boot options.
- Install and configure a boot loader such as GRUB Legacy.
- Perform basic configuration changes for GRUB 2.
- Interact with the boot loader.

The following is a partial list of the used files, terms and utilities:

- menu.lst, grub.cfg and grub.conf
- grub-install
- grub-mkconfig
- MBR


## 102.3 Manage shared libraries
**Weight**: 1

**Description**: Candidates should be able to determine the shared libraries that executable programs depend on and install them when necessary.

Key Knowledge Areas:

- Identify shared libraries.
- Identify the typical locations of system libraries.
- Load shared libraries.

The following is a partial list of the used files, terms and utilities:

- ldd
- ldconfig
- /etc/ld.so.conf
- LD_LIBRARY_PATH


## 102.4 Use Debian package management
**Weight**: 3

**Description**: Candidates should be able to perform package management using the Debian package tools.

Key Knowledge Areas:

- Install, upgrade and uninstall Debian binary packages.
- Find packages containing specific files or libraries which may or may not be installed.
- Obtain package information like version, content, dependencies, package integrity and installation status (whether or not the package is installed).
- Awareness of apt.

The following is a partial list of the used files, terms and utilities:

- /etc/apt/sources.list
- dpkg
- dpkg-reconfigure
- apt-get
- apt-cache


## 102.5 Use RPM and YUM package management
**Weight：**  3

**Description**: Candidates should be able to perform package management using RPM, YUM and Zypper.

Key Knowledge Areas:

- Install, re-install, upgrade and remove packages using RPM, YUM and Zypper.
- Obtain information on RPM packages such as version, status, dependencies, integrity and signatures.
- Determine what files a package provides, as well as find which package a specific file comes from.
- Awareness of dnf.

The following is a partial list of the used files, terms and utilities:

- rpm
- rpm2cpio
- /etc/yum.conf
- /etc/yum.repos.d/
- yum
- zypper


## 102.6 Linux as a virtualization guest
**Weight**: 1

**Description**: Candidates should understand the implications of virtualization and cloud computing on a Linux guest system.

Key Knowledge Areas:

- Understand the general concept of virtual machines and containers.
- Understand common elements virtual machines in an IaaS cloud, such as computing instances, block storage and networking.
- Understand unique properties of a Linux system which have to changed when a system is cloned or used as a template.
- Understand how system images are used to deploy virtual machines, cloud instances and containers.
- Understand Linux extensions which integrate Linux with a virtualization product.
- Awareness of cloud-init.

The following is a partial list of the used files, terms and utilities:

- Virtual machine
- Linux container
- Application container
- Guest drivers
- SSH host keys
- D-Bus machine id
