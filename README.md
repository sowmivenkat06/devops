Linux, Windows, Virtual Machines & Basic Commands
Windows Operating System

Windows is a commercial operating system developed by Microsoft and is widely used in personal and enterprise computers. It is GUI-based, beginner friendly, and mainly focused on desktop applications. Command-line operations are performed using Command Prompt or PowerShell. Customization is limited compared to Linux and it is licensed (paid).

Linux Operating System

Linux is a free and open-source operating system commonly used in servers, cloud platforms, cybersecurity, and DevOps. It is lightweight, stable, secure, and highly customizable. Many tasks are performed using the terminal. Linux comes in multiple distributions such as Ubuntu, CentOS, and Red Hat.

Linux vs Windows

Windows is mainly desktop-oriented, easier for general users, and has moderate security. Linux is preferred in server and DevOps environments because of its stability, strong security, automation support, and flexibility.

Virtual Machine (VM)

A Virtual Machine is a software computer running inside your real computer. It allows multiple operating systems to run on the same hardware. For example, Ubuntu can run inside Windows using VMware or VirtualBox. VMs are useful in DevOps for testing, isolation, and practicing Linux without affecting the host system.

Important VM Terms

A hypervisor is the software that creates VMs (like VMware or VirtualBox). The host OS is the main operating system of the physical machine, and the guest OS is the OS installed inside the VM.

In networking, NAT lets the VM share the host’s internet, while Bridged mode gives the VM its own IP address on the same network.

What is WSL

WSL (Windows Subsystem for Linux) allows Linux tools and commands to run directly on Windows without a full virtual machine. It is lightweight, faster, and easy to set up, but provides less isolation compared to a VM.

VMware Workstation

VMware Workstation Pro is virtualization software that helps create and manage virtual machines. After installing it, you can load an operating system ISO (like Ubuntu) and run it as a separate environment inside your Windows machine.

Before installation, features like Hyper-V, Virtual Machine Platform, Windows Hypervisor Platform, Windows Sandbox, and WSL should be disabled. Hardware virtualization must also be enabled in BIOS.

Ubuntu Server Installation (Overview)

Create a new VM, attach the Ubuntu Server ISO, choose Linux → Ubuntu 64-bit, assign RAM and CPU, and create a virtual disk. During installation, select language, keyboard, default network, and “use entire disk” (this affects only the virtual disk). Create username and password, optionally install OpenSSH, wait for installation, and reboot. After login, update the system using:

sudo apt update
sudo apt upgrade

Linux Commands

Linux commands help manage files, software, users, and system processes.

You can check your current directory using pwd, list files with ls, and change folders using cd. Directories are created with mkdir, and files can be created with touch. Files or folders are copied using cp, moved or renamed using mv, and deleted using rm.

To read files, use cat, less, head, or tail. Editing can be done using editors like nano or vi.

Searching text is done using grep, and files can be found using find or locate.

Permissions are controlled with chmod, ownership with chown, and can be viewed using ls -l.

System information like memory, disk, and processes can be checked using commands such as uname, df, free, top, and whoami.

For networking, ip a shows IP details and ping checks connectivity.

Package Management (Ubuntu)

Software installation and updates are handled with APT.
sudo apt update refreshes package lists, and sudo apt upgrade installs the newest versions. Packages can be installed using sudo apt install and removed using sudo apt remove.

Process & System Control

Running processes can be viewed using ps. A process can be stopped using kill. The system can be restarted with reboot or powered off with shutdown.

vi Editor

vi is a terminal text editor. Press i to insert text, Esc to exit insert mode, :w to save, :q to quit, and :wq to save and quit.

LTS (Long Term Support)

LTS versions of Ubuntu receive updates and security fixes for many years. They are recommended for production and server environments because of their reliability and stability.

rm -rf

rm means remove. The -r option deletes directories recursively and -f forces deletion without confirmation. This command is powerful and must be used carefully.
