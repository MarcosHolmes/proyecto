# Title 

Install Docker Desktop on Linux

### Prerequisites

To install Docker Desktop successfully, your Linux host must meet the following general requirements:

    64-bit kernel and CPU support for virtualization.
    KVM virtualization support. Follow the KVM virtualization support instructions to check if the KVM kernel modules are enabled and how to provide access to the kvm device.
    QEMU must be version 5.2 or newer. We recommend upgrading to the latest version.
    systemd init system.
    Gnome, KDE, or MATE Desktop environment.
        For many Linux distros, the Gnome environment does not support tray icons. To add support for tray icons, you need to install a Gnome extension. For example, AppIndicator.
    At least 4 GB of RAM.
    Enable configuring ID mapping in user namespaces, see File sharing.

Docker Desktop for Linux runs a Virtual Machine (VM). 

### Installing

To install Docker Desktop successfully, you must:

    Meet the system requirements
    Have a 64-bit version of either Ubuntu Jammy Jellyfish 22.04 (LTS) or Ubuntu Impish Indri 21.10. Docker Desktop is supported on x86_64 (or amd64) architecture.
    
	For non-Gnome Desktop environments, gnome-terminal must be installed: 

		sudo apt install gnome-terminal

Install Docker Desktop

Recommended approach to install Docker Desktop on Ubuntu:

    Set up Docker’s package repository.

    Download latest DEB package.

    Install the package with apt as follows:
	sudo apt-get update
	sudo apt-get install ./docker-desktop-<version>-<arch>.deb
	
	Launch Docker Desktop

To start Docker Desktop for Linux, search Docker Desktop on the Applications menu and open it. This launches the Docker menu icon and opens the Docker Dashboard, reporting the status of Docker Desktop.

Alternatively, open a terminal and run:

	systemctl --user start docker-desktop
	
To enable Docker Desktop to start on login, from the Docker menu, select Settings > General > Start Docker Desktop when you log in.

Alternatively, open a terminal and run:
	systemctl --user enable docker-desktop
		
## Built With

https://docs.docker.com/desktop/install/ubuntu/

## Authors

Marcos Aguilar 

