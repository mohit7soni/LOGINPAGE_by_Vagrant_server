financeIAC
This project uses Vagrant and VirtualBox to automate the provisioning of a CentOS Stream 9 virtual machine for web application deployment.
The VM is configured with:

Apache HTTP Server (httpd)
Wget, Unzip, and Zip utilities
Automatic download and deployment of a sample web template from Tooplate
Private and public network interfaces for flexible access
Features
Automated provisioning: Installs and configures Apache, downloads a web template, and sets up the web server automatically.
Network configuration: Sets up both private and public networks for development and testing.
Easy cleanup: Temporary files are removed after provisioning.

Usage
Clone this repository.
Run vagrant up in the project directory.
Access the deployed web application via the VM’s IP address.



Features
Automated VM Provisioning:
Uses Vagrant and VirtualBox to spin up a CentOS Stream 9 VM with a single command.
Web Server Setup:
Installs Apache (httpd) and required utilities (wget, unzip, zip).
Sample Web Application:
Automatically downloads and deploys a sample HTML template from Tooplate.
Network Configuration:
Sets up both private and public networks for flexible access.
Clean Provisioning:
Removes temporary files after setup.
Prerequisites
Vagrant
VirtualBox
Git (optional, for cloning the repo)
Getting Started
Clone the repository:

Start the VM:

Access the Web Application:

Open your browser and go to:
http://192.168.56.70
Project Structure
financeIAC/
├── Vagrantfile
└── (other files and folders as needed)

Vagrantfile: Main configuration for VM provisioning and setup.
How It Works
The Vagrantfile provisions a CentOS Stream 9 VM and runs the following steps automatically:

Installs Apache, wget, unzip, and zip.
Starts and enables the Apache service.
Downloads a sample web template.
Unzips and copies the template to /var/www/html/.
Restarts Apache and cleans up temporary files.
Customization
Change the Web Template:
Edit the URL in the Vagrantfile to use a different template.
